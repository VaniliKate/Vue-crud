<template>
  <div class="container">
    <HeaderComp title="App" />
    <TasksComp :tasks="tasks" />
  </div>
</template>

<script>

import HeaderComp from './components/HeaderComp.vue'
import TasksComp from './components/TasksComp.vue'


export default {
  name: "App",
  components: {
    HeaderComp,
    TasksComp
    
  },
  data(){
    return{
      tasks: []
    }
  },
  created(){
    this.tasks = [
      {
        "id": 1,
        "company_name": "My awesome Company",
        "contact_firstname": "Jane",
        "contact_lastname": "Doe",
        "contact_email": "jdoe@awesome.com",
        "acquired_on": "2021-04-03",
        "customer_status": "active"
      },
      {
        "id": 2,
        "company_name": "Company ABC",
        "contact_firstname": "Sarah",
        "contact_lastname": "Jane",
        "contact_email": "sjane@coabc.com",
        "acquired_on": "2021-06-03",
        "customer_status": "active"
      },
      {
        "id": 3,
        "company_name": "Company xYZ",
        "contact_firstname": "Tim",
        "contact_lastname": "Hane",
        "contact_email": "thane@coxyz.com",
        "acquired_on": "2020-12-03",
        "customer_status": "active"
      },
      {
        "id": 4,
        "company_name": "Video Production Consulting",
        "contact_firstname": "Miriam",
        "contact_lastname": "Doe",
        "contact_email": "mdoe@vidprod.com",
        "acquired_on": "2020-07-05",
        "customer_status": "inactive"
      },
      {
        "id": 5,
        "company_name": "Code Writers",
        "contact_firstname": "Jill",
        "contact_lastname": "Wade",
        "contact_email": "jwade@codewrit.com",
        "acquired_on": "2020-04-03",
        "customer_status": "active"
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