<template>
  <div>
    <h1>Часто задаваемые вопросы</h1>
    <el-card v-for="faq in faqs" :key="faq.id">
      <h2>{{ faq.question }}</h2>
      <p>{{ faq.answer }}</p>
    </el-card>
  </div>
</template>

<script>
import { ref } from 'vue';
import { faqs } from "@/data.js";

export default {
  data() {
    return {
      faqs: faqs
    };
  }
};
</script>
