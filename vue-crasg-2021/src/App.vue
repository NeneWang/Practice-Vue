<template>
  <div class="container">
    <Header title="Hello" />
    <Tasks :tasks="tasks"  />
  </div>
</template>

<script>
import Header from "./components/Header";
import Tasks from './components/Tasks'

export default {
  name: "App",
  components: {
    Header,
    Tasks
  },
  data(){
    return {
      tasks: []
      }
  },
  created(){
    this.tasks = [
 {
   "id": 1,
   "text": "Doctors Appointment",
   "day": "March 1st at 2:30",
   "reminder": true
 },
 {
   "id": 2,
   "text": "Not Doctors",
   "day": "March 1st at 2:31",
   "reminder": true
 },
 {
   "id": 3,
   "text": "Maincraft Appointment",
   "day": "March 1st at 2:32",
   "reminder": false
 },
 {
   "id": 4,
   "text": "What am I doing with my life",
   "day": "March 1st at 2:33",
   "reminder": true
 },
 {
   "id": 5,
   "text": "Data Structures",
   "day": "March 1st at 2:34",
   "reminder": false
 },
 {
   "id": 6,
   "text": "Reformat",
   "day": "March 1st at 2:35",
   "reminder": false
 },
 {
   "id": 7,
   "text": "GG Yasuo",
   "day": "March 1st at 2:36",
   "reminder": true
 }
]
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400&display=swap");
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: "Poppins", sans-serif;
}
.container {
  max-width: 500px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 1px solid steelblue;
  padding: 30px;
  border-radius: 5px;
}
.btn {
  display: inline-block;
  background: #000;
  color: #fff;
  border: none;
  padding: 10px 20px;
  margin: 5px;
  border-radius: 5px;
  cursor: pointer;
  text-decoration: none;
  font-size: 15px;
  font-family: inherit;
}
.btn:focus {
  outline: none;
}
.btn:active {
  transform: scale(0.98);
}
.btn-block {
  display: block;
  width: 100%;
}
</style>
