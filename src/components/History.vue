<template>
    <div>
      <h1>История проекта</h1>
      <ul>
        <li v-for="event in history" :key="event.id">
          <h2>{{ event.date }}</h2>
          <h3>{{ event.title }}</h3>
          <p>{{ event.value }}</p>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  import { history } from "@/data.js";
  
  export default {
    data() {
      return {
        history: history
      };
    }
  };
  </script>
  