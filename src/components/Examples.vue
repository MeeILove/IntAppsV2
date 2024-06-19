<template>
    <section id="examples">
      <h2>Примеры использования</h2>
      <div class="example-list">
        <div class="example-item" v-for="example in examples" :key="example.id">
          <img :src="require(`@/assets/${example.image}`)" :alt="example.title" />
          <h3>{{ example.title }}</h3>
          <p>{{ example.description }}</p>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        examples: [
          { id: 1, image: 'finance.jpg', title: 'Финансовый сектор', description: 'Интеллектуальные приложения в финансах помогают в анализе больших данных и прогнозировании рынка.' },
          { id: 2, image: 'medicine.jpg', title: 'Медицина', description: 'В медицине ИИ используется для диагностики заболеваний и персонализированного лечения.' },
          { id: 3, image: 'manufacturing.jpg', title: 'Производство', description: 'Интеллектуальные приложения помогают оптимизировать производственные процессы и улучшить качество продукции.' }
        ],
      };
    },
  };
  </script>
  
  <style>
  #examples {
    padding: 50px 20px;
    background: #f9f9f9;
    text-align: center;
  }
  .example-list {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }
  .example-item {
    width: 30%;
    margin: 20px 0;
  }
  .example-item img {
    width: 100%;
    height: auto;
  }
  .example-item h3 {
    font-size: 24px;
    margin: 10px 0;
  }
  .example-item p {
    font-size: 16px;
  }
  </style>
  