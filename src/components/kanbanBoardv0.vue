<template>
    <div class="kanban-container">
      <header class="kanban-header">
        <h1>Welcome to the Task Management Kanban Board</h1>
        <div class="project-filter">
          <label for="project">Filter by Project:</label>
          <select v-model="selectedProject" @change="fetchTasks">
            <option value="">All Projects</option>
            <option v-for="project in projects" :key="project.id" :value="project.id">{{ project.name }}</option>
          </select>
        </div>
      </header>
      <div class="kanban-board">
        <div class="column" v-for="status in statuses" :key="status" :class="statusClass(status)">
          <h2>{{ statusLabels[status] }}</h2>
          <div class="task" v-for="task in filteredTasks(status)" :key="task.id">
            <div class="task-header">
              <h3>{{ task.title }}</h3>
              <span class="priority" :class="priorityClass(task.priority)">{{ task.priority }}</span>
            </div>
            <div class="task-details">
              <p><strong>Reporter:</strong> {{ task.reporter.name }}</p>
              <p><strong>Start Date:</strong> {{ task.start_date }}</p>
              <p><strong>Expected End Date:</strong> {{ task.expected_end_date }}</p>
            </div>
            <div class="task-footer">
              <span class="status-label" :class="statusLabelClass(task.status)">{{ statusLabels[task.status] }}</span>
              <a v-if="task.jira_ticket_link" :href="task.jira_ticket_link" target="_blank" class="jira-link">JIRA</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  import axios from 'axios';
  
  export default {
    data() {
      return {
        tasks: [],
        projects: [],
        selectedProject: '',
        statuses: ['not_started', 'in_progress', 'completed'],
        statusLabels: {
          not_started: 'Not Started',
          in_progress: 'In Progress',
          completed: 'Done'
        }
      };
    },
    created() {
      this.fetchProjects();
      this.fetchTasks();
    },
    methods: {
      fetchProjects() {
        axios.get('http://localhost:8000/api/projects/')  // Assuming you have an endpoint for projects
          .then(response => {
            this.projects = response.data;
          })
          .catch(error => {
            console.log(error);
          });
      },
      fetchTasks() {
        let url = 'http://localhost:8000/api/tasks/';
        if (this.selectedProject) {
          url += `?project=${this.selectedProject}`;
        }
        axios.get(url)
          .then(response => {
            this.tasks = response.data;
          })
          .catch(error => {
            console.log(error);
          });
      },
      filteredTasks(status) {
        return this.tasks.filter(task => task.status === status);
      },
      statusClass(status) {
        return {
          'not-started': status === 'not_started',
          'in-progress': status === 'in_progress',
          'completed': status === 'completed'
        };
      },
      statusLabelClass(status) {
        return {
          'status-label-gray': status === 'not_started',
          'status-label-yellow': status === 'in_progress',
          'status-label-green': status === 'completed'
        };
      },
      priorityClass(priority) {
        return {
          'priority-high': priority === 'high',
          'priority-medium': priority === 'medium',
          'priority-low': priority === 'low'
        };
      },
    },
  };
  </script>
  
  <style>
  .kanban-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 20px;
  }
  
  .kanban-header {
    text-align: center;
    margin-bottom: 20px;
  }
  
  .project-filter {
    margin-top: 10px;
  }
  
  .kanban-board {
    display: flex;
    justify-content: space-between;
  }
  
  .column {
    width: 30%;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  
  .column h2 {
    text-align: center;
    margin-bottom: 20px;
    padding: 10px;
    border-radius: 5px;
  }
  
  .task {
    background-color: #fff;
    padding: 15px;
    margin-bottom: 15px;
    border-radius: 5px;
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
    transition: transform 0.2s;
  }
  
  .task:hover {
    transform: scale(1.02);
  }
  
  .task-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
  }
  
  .priority {
    padding: 4px 8px;
    border-radius: 3px;
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
  }
  
  .priority-high {
    background-color: #dc3545;
    color: #fff;
  }
  
  .priority-medium {
    background-color: #ffc107;
    color: #333;
  }
  
  .priority-low {
    background-color: #28a745;
    color: #fff;
  }
  
  .task-details {
    margin-bottom: 10px;
  }
  
  .task-footer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 10px;
    font-size: 12px;
  }
  
  .status-label {
    padding: 4px 8px;
    border-radius: 3px;
    font-size: 12px;
    font-weight: bold;
    text-transform: uppercase;
  }
  
  .status-label-gray {
    background-color: #6c757d;
    color: #fff;
  }
  
  .status-label-yellow {
    background-color: #ffc107;
    color: #333;
  }
  
  .status-label-green {
    background-color: #28a745;
    color: #fff;
  }
  
  .jira-link {
    color: #007bff;
    text-decoration: none;
  }
  
  .jira-link:hover {
    text-decoration: underline;
  }
  </style>
  