<template>
    <!-- Working version of https://dribbble.com/shots/14552329--Exploration-Task-Management-Dashboard -->
<div class='app'>
  <main class='project'>
    <div class='project-info'>
      <h1>Homepage Design</h1>
      <div class='project-participants'>
        <span></span>
        <span></span>
        <span></span>
        <button class='project-participants__add'>Add Participant</button>
          
        </div>
    </div>
    <div class='project-tasks'>
      <div class='project-column'>
        <div class='project-column-heading'>
          <h2 class='project-column-heading__title'>Task Ready</h2><button class='project-column-heading__options'><i class="fas fa-ellipsis-h"></i></button>
        </div>
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--copyright'>Copywriting</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Konsep hero title yang menarik</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>3</span>
            <span><i class="fas fa-paperclip"></i>7</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
                <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--design'>UI Design</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Icon di section our services</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>2</span>
            <span><i class="fas fa-paperclip"></i>5</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
                <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--copyright'>Copywriting</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Konsep hero title yang menarik</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>2</span>
            <span><i class="fas fa-paperclip"></i>3</span>
            <span class='task__owner'></span>
          </div>
        </div>
      </div>
      <div class='project-column'><div class='project-column-heading'>
          <h2 class='project-column-heading__title'>In Progress</h2><button class='project-column-heading__options'><i class="fas fa-ellipsis-h"></i></button>
        </div>
          
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--design'>UI Design</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Replace lorem ipsum text in the final designs</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>5</span>
            <span><i class="fas fa-paperclip"></i>5</span> 
            <span class='task__owner'></span>
          </div>
        </div>
        
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--illustration'>Illustration</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Create and generate the custom SVG illustrations.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>8</span>
            <span><i class="fas fa-paperclip"></i>7</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--copyright'>Copywriting</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Proof read the legal page and check for and loopholes</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>12</span>
            <span><i class="fas fa-paperclip"></i>11</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--illustration'>Illustration</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Create the landing page graphics for the hero slider.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>4</span>
            <span><i class="fas fa-paperclip"></i>8</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
        </div>
      <div class='project-column'><div class='project-column-heading'>
          <h2 class='project-column-heading__title'>Needs Review</h2><button class='project-column-heading__options'><i class="fas fa-ellipsis-h"></i></button>
        </div>
          
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--copyright'>Copywriting</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Check the company we copied doesn't think we copied them.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>4</span>
            <span><i class="fas fa-paperclip"></i>0</span>
            <span class='task__owner'></span>
          </div>
        </div>
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--design'>UI Design</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Design the about page.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>0</span>
            <span><i class="fas fa-paperclip"></i>5</span>
            <span class='task__owner'></span>
          </div>
        </div>
        <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--illustration'>Illustration</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Move that one image 5px down to make Phil Happy.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>2</span>
            <span><i class="fas fa-paperclip"></i>2</span>
            <span class='task__owner'></span>
          </div>
        </div>
        </div>
      <div class='project-column'><div class='project-column-heading'>
          <h2 class='project-column-heading__title'>Done</h2><button class='project-column-heading__options'><i class="fas fa-ellipsis-h"></i></button>
        </div>
        
         <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--illustration'>Illustration</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Send Advert illustrations over to production company.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>12</span>
            <span><i class="fas fa-paperclip"></i>5</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
         <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--illustration'>Illustration</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Dawn wants to move the text 3px to the right.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>3</span>
            <span><i class="fas fa-paperclip"></i>7</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
         <div class='task' draggable='true'>
          <div class='task__tags'><span class='task__tag task__tag--copyright'>Copywriting</span><button class='task__options'><i class="fas fa-ellipsis-h"></i></button></div>
          <p>Amend the contract details.</p>
          <div class='task__stats'>
            <span><time datetime="2021-11-24T20:00:00"><i class="fas fa-flag"></i>Nov 24</time></span>
            <span><i class="fas fa-comment"></i>8</span>
            <span><i class="fas fa-paperclip"></i>16</span>
            <span class='task__owner'></span>
          </div>
        </div>
        
        </div>
      
    </div>
  </main>
  <aside class='task-details'>
    <div class='tag-progress'>
      <h2>Task Progress</h2>
      <div class='tag-progress'>
        <p>Copywriting <span>3/8</span></p>
        <progress class="progress progress--copyright" max="8" value="3"> 3 </progress>
      </div>
      <div class='tag-progress'>
        <p>Illustration <span>6/10</span></p>
        <progress class="progress progress--illustration" max="10" value="6"> 6 </progress>
      </div>
      <div class='tag-progress'>
        <p>UI Design <span>2/7</span></p>
        <progress class="progress progress--design" max="7" value="2"> 2 </progress>
      </div>
    </div>
    <div class='task-activity'>
      <h2>Recent Activity</h2>
      <ul>
        <li>
          <span class='task-icon task-icon--attachment'><i class="fas fa-paperclip"></i></span>
          <b>Andrea </b>uploaded 3 documents
          <time datetime="2021-11-24T20:00:00">Aug 10</time>
        </li>
          <li>
              <span class='task-icon task-icon--comment'><i class="fas fa-comment"></i></span>
          <b>Karen </b> left a comment
          <time datetime="2021-11-24T20:00:00">Aug 10</time>
        </li>
         <li>
             <span class='task-icon task-icon--edit'><i class="fas fa-pencil-alt"></i></span>
          <b>Karen </b>uploaded 3 documents
          <time datetime="2021-11-24T20:00:00">Aug 11</time>
        </li>
          <li>
              <span class='task-icon task-icon--attachment'><i class="fas fa-paperclip"></i></span>
          <b>Andrea </b>uploaded 3 documents
          <time datetime="2021-11-24T20:00:00">Aug 11</time>
        </li>
         <li>
             <span class='task-icon task-icon--comment'><i class="fas fa-comment"></i></span>
          <b>Karen </b> left a comment
          <time datetime="2021-11-24T20:00:00">Aug 12</time>
        </li>
      </ul>
    </div>
  </aside>
</div>
  </template>
  
  <script>
export default {
  mounted() {
    document.addEventListener('DOMContentLoaded', () => {
      let dragSrcEl = null;
      let items = document.querySelectorAll('.task');

      function handleDragStart(event) {
        event.target.style.opacity = '0.1';
        event.target.style.border = '3px dashed #c4cad3';

        dragSrcEl = event.target;

        event.dataTransfer.effectAllowed = 'move';
        event.dataTransfer.setData('text/html', event.target.innerHTML);
      }

      function handleDragOver(event) {
        if (event.preventDefault) {
          event.preventDefault();
        }

        event.dataTransfer.dropEffect = 'move';

        return false;
      }

      function handleDragEnter(event) {
        event.target.classList.add('task-hover');
      }

      function handleDragLeave(event) {
        event.target.classList.remove('task-hover');
      }

      function handleDrop(event) {
        if (event.stopPropagation) {
          event.stopPropagation(); // stops the browser from redirecting.
        }

        if (dragSrcEl !== event.target) {
          dragSrcEl.innerHTML = event.target.innerHTML;
          event.target.innerHTML = event.dataTransfer.getData('text/html');
        }

        return false;
      }

      function handleDragEnd(event) {
        event.target.style.opacity = '1';
        event.target.style.border = 'none';

        items.forEach(function (item) {
          item.classList.remove('task-hover');
        });
      }

      items.forEach(function (item) {
        item.addEventListener('dragstart', handleDragStart, false);
        item.addEventListener('dragenter', handleDragEnter, false);
        item.addEventListener('dragover', handleDragOver, false);
        item.addEventListener('dragleave', handleDragLeave, false);
        item.addEventListener('drop', handleDrop, false);
        item.addEventListener('dragend', handleDragEnd, false);
      });
    });
  }
};
</script>

<style>
:root {
  --bg:#ebf0f7;
  --header:#fbf4f6;
  --text:#2e2e2f;
  --white:#ffffff;
  --light-grey:#c4cad3;
  --tag-1:#ceecfd;
  --tag-1-text:#2e87ba;
  --tag-2:#d6ede2;
  --tag-2-text:#13854e;
  --tag-3:#ceecfd;
  --tag-3-text:#2d86ba;
  --tag-4:#f2dcf5;
  --tag-4-text:#a734ba;
  --purple:#7784ee;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

body {
  color: var(--text);
}

.app {
  background-color: var(--bg);
  width: 100%;
  min-height: 100vh;
}

h1 {
  font-size: 30px;
}

.project {
  padding: 2rem;
  max-width: 75%;
  width: 100%;
  display: inline-block;
}
.project-info {
  padding: 2rem 0;
  display: flex;
  width: 100%;
  justify-content: space-between;
  align-items: center;
}
.project-participants {
  display: flex;
  align-items: center;
}
.project-participants span, .project-participants__add {
  width: 30px;
  height: 30px;
  display: inline-block;
  background: var(--purple);
  border-radius: 100rem;
  margin: 0 0.2rem;
}
.project-participants__add {
  background: transparent;
  border: 1px dashed #969696;
  font-size: 0;
  cursor: pointer;
  position: relative;
}
.project-participants__add:after {
  content: "+";
  font-size: 15px;
  color: #969696;
}
.project-tasks {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  width: 100%;
  grid-column-gap: 1.5rem;
}
.project-column-heading {
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.project-column-heading__title {
  font-size: 20px;
}
.project-column-heading__options {
  background: transparent;
  color: var(--light-grey);
  font-size: 18px;
  border: 0;
  cursor: pointer;
}

.task {
  cursor: move;
  background-color: var(--white);
  padding: 1rem;
  border-radius: 8px;
  width: 100%;
  box-shadow: rgba(99, 99, 99, 0.1) 0px 2px 8px 0px;
  margin-bottom: 1rem;
  border: 3px dashed transparent;
}
.task:hover {
  box-shadow: rgba(99, 99, 99, 0.3) 0px 2px 8px 0px;
  border-color: rgba(162, 179, 207, 0.2) !important;
}
.task p {
  font-size: 15px;
  margin: 1.2rem 0;
}
.task__tag {
  border-radius: 100px;
  padding: 2px 13px;
  font-size: 12px;
}
.task__tag--copyright {
  color: var(--tag-4-text);
  background-color: var(--tag-4);
}
.task__tag--design {
  color: var(--tag-3-text);
  background-color: var(--tag-3);
}
.task__tag--illustration {
  color: var(--tag-2-text);
  background-color: var(--tag-2);
}
.task__tags {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.task__options {
  background: transparent;
  border: 0;
  color: var(--light-grey);
  font-size: 17px;
}
.task__stats {
  position: relative;
  width: 100%;
  color: var(--light-grey);
  font-size: 12px;
}
.task__stats span:not(:last-of-type) {
  margin-right: 1rem;
}
.task__stats svg {
  margin-right: 5px;
}
.task__owner {
  width: 25px;
  height: 25px;
  border-radius: 100rem;
  background: var(--purple);
  position: absolute;
  display: inline-block;
  right: 0;
  bottom: 0;
}

.task-hover {
  border: 3px dashed var(--light-grey) !important;
}

.task-details {
  width: 24%;
  border-left: 1px solid #d9e0e9;
  display: inline-block;
  height: 100%;
  vertical-align: top;
  padding: 3rem 2rem;
}

.tag-progress {
  margin: 1.5rem 0;
}
.tag-progress h2 {
  font-size: 16px;
  margin-bottom: 1rem;
}
.tag-progress p {
  display: flex;
  width: 100%;
  justify-content: space-between;
}
.tag-progress p span {
  color: #b4b4b4;
}
.tag-progress .progress {
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
       appearance: none;
  border: none;
  border-radius: 10px;
  height: 10px;
}
.tag-progress .progress::-webkit-progress-bar, .tag-progress .progress::-webkit-progress-value {
  border-radius: 10px;
}
.tag-progress .progress--copyright::-webkit-progress-bar {
  background-color: #ecd8e6;
}
.tag-progress .progress--copyright::-webkit-progress-value {
  background: #d459e8;
}
.tag-progress .progress--illustration::-webkit-progress-bar {
  background-color: #dee7e3;
}
.tag-progress .progress--illustration::-webkit-progress-value {
  background-color: #46bd84;
}
.tag-progress .progress--design::-webkit-progress-bar {
  background-color: #d8e7f4;
}
.tag-progress .progress--design::-webkit-progress-value {
  background-color: #08a0f7;
}

.task-activity h2 {
  font-size: 16px;
  margin-bottom: 1rem;
}
.task-activity li {
  list-style: none;
  margin: 1rem 0;
  padding: 0rem 1rem 1rem 3rem;
  position: relative;
}
.task-activity time {
  display: block;
  color: var(--light-grey);
}

.task-icon {
  width: 30px;
  height: 30px;
  border-radius: 100rem;
  position: absolute;
  top: 0;
  left: 0;
  display: flex;
  align-items: center;
  justify-content: center;
}
.task-icon svg {
  font-size: 12px;
  color: var(--white);
}
.task-icon--attachment {
  background-color: #fba63c;
}
.task-icon--comment {
  background-color: #5dc983;
}
.task-icon--edit {
  background-color: #7784ee;
}

@media only screen and (max-width: 1300px) {
  .project {
    max-width: 100%;
  }

  .task-details {
    width: 100%;
    display: flex;
  }

  .tag-progress,
.task-activity {
    flex-basis: 50%;
    background: var(--white);
    padding: 1rem;
    border-radius: 8px;
    margin: 1rem;
  }
}
@media only screen and (max-width: 1000px) {
  .project-column:nth-child(2),
.project-column:nth-child(3) {
    display: none;
  }

  .project-tasks {
    grid-template-columns: 1fr 1fr;
  }
}
@media only screen and (max-width: 600px) {
  .project-column:nth-child(4) {
    display: none;
  }

  .project-tasks {
    grid-template-columns: 1fr;
  }

  .task-details {
    flex-wrap: wrap;
    padding: 3rem 1rem;
  }

  .tag-progress,
.task-activity {
    flex-basis: 100%;
  }

  h1 {
    font-size: 25px;
  }
}
</style>

  
  <!-- <style>
  :root {
  --bg:#ebf0f7;
  --header:#fbf4f6;
  --text:#2e2e2f;
  --white:#ffffff;
  --light-grey:#c4cad3; 
  --tag-1:#ceecfd;
  --tag-1-text:#2e87ba;
  --tag-2:#d6ede2;
  --tag-2-text:#13854e;
  --tag-3:#ceecfd;
  --tag-3-text:#2d86ba;
  --tag-4:#f2dcf5;
  --tag-4-text:#a734ba;
  --purple:#7784ee;
}
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Poppins', sans-serif;
  
}

body {
  color:var(--text);
}

@mixin display {
  display:flex;
  align-items:center;
}

.app {
  background-color:var(--bg);
  width:100%;
  min-height:100vh;
}

h1 {
  font-size:30px;
}
.project {
  padding:2rem;
  max-width:75%;
  width:100%;
  display:inline-block;
  
  &-info {
    padding:2rem 0;
    display:flex;
    width:100%;
    justify-content:space-between;
    align-items:center;
  }
  &-participants {
    @include display;
    span,
    &__add{
      width:30px;
      height:30px;
      display:inline-block;
      background:var(--purple);
      border-radius:100rem;
      margin:0 .2rem; 
    }
    &__add {
     background:transparent;
     border:1px dashed rgb(150,150,150);
     font-size:0;
     cursor:pointer;
     position:relative;
      
      &:after {
        content:'+';
        font-size:15px;
        color:rgb(150,150,150);
        
      }
    }
  }
  
  &-tasks {
    display:grid;
    grid-template-columns:repeat(4,1fr);
    width:100%;
    grid-column-gap:1.5rem;
  }
  &-column {
    
    &-heading {
      margin-bottom:1rem;
      @include display;
      justify-content:space-between;
      &__title {
        font-size:20px;
 
      }
      &__options {
        background:transparent;
        color:var(--light-grey);
        font-size:18px;
        border:0;
          cursor:pointer;
      }
    }
  }
}

.task {
  cursor:move;
  background-color:var(--white);
  padding:1rem;
  border-radius:8px;
  width:100%;
  box-shadow: rgba(99, 99, 99, 0.1) 0px 2px 8px 0px;
  margin-bottom:1rem;
  border:3px dashed transparent;
  
  &:hover {
     box-shadow: rgba(99, 99, 99, 0.3) 0px 2px 8px 0px;
    border-color:rgba(162,179,207,.2)!important;
  }
  
  p {
    font-size:15px;
    margin:1.2rem 0;
  }
  &__tag {
    border-radius:100px;
    padding:2px 13px;
    font-size:12px;
    
    &--copyright {
      color:var(--tag-4-text);
      background-color:var(--tag-4);
    }
    &--design {
       color:var(--tag-3-text);
      background-color:var(--tag-3);
    }
    &--illustration {
      color:var(--tag-2-text);
      background-color:var(--tag-2);
    }
    
  }
  &__tags { 
    width:100%;
    @include display;
    justify-content:space-between;
  }
  
  &__options {
      background:transparent; 
      border:0;
    color:var(--light-grey);
    font-size:17px;
    }
  
  &__stats {
    
    position:relative;
    width:100%;
    color:var(--light-grey);
    
    font-size:12px;
    span:not(:last-of-type){
      margin-right:1rem;
    }
    svg {
      margin-right:5px;
    }
  }
  
  &__owner {
    width:25px;
    height:25px;
    border-radius:100rem;
    background:var(--purple);
    position:absolute;
    display:inline-block;
    right:0;
    bottom:0;
    
  }
}

.task-hover {
border:3px dashed var(--light-grey)!important;
}
.task-details {
  width:24%;
  border-left:1px solid #d9e0e9;
  display:inline-block;
  height:100%;
  vertical-align:top;
  padding:3rem 2rem;
}

.tag-progress {
  margin:1.5rem 0;
  h2 {
    font-size:16px;
    margin-bottom:1rem;
  }
  p {
    display:flex;
    width:100%;
    justify-content:space-between;
    
    span {
      color:rgb(180,180,180);
    }
  }
  .progress {
    width:100%;
    -webkit-appearance: none;
    appearance: none;
    border:none;
    border-radius:10px;
    height:10px;
    
    &::-webkit-progress-bar,
    &::-webkit-progress-value {
      border-radius:10px;
    }
    &--copyright {
      &::-webkit-progress-bar {
      background-color:#ecd8e6;
    }
    
    &::-webkit-progress-value {
      background:#d459e8
    }
    }
    
        &--illustration {
      &::-webkit-progress-bar {
      background-color:#dee7e3;
      
    }
    
    &::-webkit-progress-value {
      background-color:#46bd84;
    }
    }
    
        &--design {
      &::-webkit-progress-bar {
      
      background-color:#d8e7f4;
    }
    
    &::-webkit-progress-value {
      background-color:#08a0f7;
    }
    }
    

  }
}

.task-activity {
   h2 {
    font-size:16px;
    margin-bottom:1rem;
  }
  
  li {
    list-style:none;
    margin:1rem 0;
    padding:0rem 1rem 1rem 3rem;
    position:relative;
  }
  time {
    display:block;
    color:var(--light-grey);
  }
}

.task-icon {
  width:30px;
  height:30px;
  border-radius:100rem;
  position:absolute;
  top:0;
  left:0;
  @include display;
  justify-content:center;
  

  svg {
    font-size:12px;
    color:var(--white);
  }
  &--attachment {
    background-color:#fba63c;
  }
  
  &--comment {
    background-color:#5dc983;
  }
  
  &--edit {
    background-color:#7784ee;
  }
 
}





@media only screen and (max-width: 1300px) {
  .project {
    max-width:100%;
  }
  .task-details {
    width:100%;
    display:flex;
  }
  .tag-progress,
  .task-activity {
    flex-basis:50%;
    background:var(--white);
    padding:1rem;
    border-radius:8px;
    margin:1rem;
  }
}

@media only screen and (max-width: 1000px) {
  .project-column:nth-child(2),
  .project-column:nth-child(3){
    display:none;
  }
  .project-tasks {
    grid-template-columns:1fr 1fr;
  }
}



@media only screen and (max-width: 600px) {
  .project-column:nth-child(4){
    display:none;
  }
  .project-tasks {
    grid-template-columns:1fr;
  }
  
  .task-details {
    flex-wrap:wrap;
    padding:3rem 1rem;
  }
  .tag-progress,
  .task-activity {
    flex-basis:100%;
  }
  h1 {
    font-size:25px;
  }
}
  </style> -->
  