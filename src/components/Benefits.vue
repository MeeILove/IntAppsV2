<template>
    <section id="benefits">
      <h2>Преимущества</h2>
      <div class="benefit-list">
        <div class="benefit-item" v-for="benefit in benefits" :key="benefit.id">
          <img :src="require(`@/assets/${benefit.icon}`)" :alt="benefit.title" />
          <h3>{{ benefit.title }}</h3>
          <p>{{ benefit.description }}</p>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        benefits: [
          { id: 1, icon: 'icon-productivity.png', title: 'Повышение продуктивности', description: 'Автоматизация рутинных задач позволяет сотрудникам фокусироваться на более важных проектах.' },
          { id: 2, icon: 'icon-cost.png', title: 'Снижение затрат', description: 'Интеллектуальные приложения помогают сократить расходы на операционные процессы.' },
          { id: 3, icon: 'icon-quality.png', title: 'Улучшение качества', description: 'Использование ИИ позволяет минимизировать ошибки и улучшить качество продукции.' }
        ],
      };
    },
  };
  </script>
  
  <style>
  #benefits {
    padding: 50px 20px;
    background: #fff;
    text-align: center;
  }
  .benefit-list {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
  }
  .benefit-item {
    width: 30%;
    margin: 20px 0;
  }
  .benefit-item img {
    width: 50px;
    height: 50px;
  }
  .benefit-item h3 {
    font-size: 24px;
    margin: 10px 0;
  }
  .benefit-item p {
    font-size: 16px;
  }
  </style>
  