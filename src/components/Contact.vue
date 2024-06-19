<template>
    <section id="contact">
      <h2>Контакты</h2>
      <form @submit.prevent="submitForm">
        <input type="text" v-model="name" placeholder="Ваше имя" required />
        <input type="email" v-model="email" placeholder="Ваш email" required />
        <textarea v-model="message" placeholder="Ваше сообщение" required></textarea>
        <button type="submit">Отправить</button>
      </form>
      <div class="map">
        <iframe src="your_google_map_link_here" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: '',
        email: '',
       ```vue
  export default {
    data() {
      return {
        name: '',
        email: '',
        message: ''
      };
    },
    methods: {
      submitForm() {
        alert(`Спасибо за ваше сообщение, ${this.name}!`);
        this.name = '';
        this.email = '';
        this.message = '';
      }
    }
  }
  </script>
  
  <style>
  #contact {
    padding: 50px 20px;
    background: #fff;
    text-align: center;
  }
  form {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  form input, form textarea {
    width: 80%;
    padding: 10px;
    margin: 10px 0;
  }
  form button {
    padding: 10px 20px;
    cursor: pointer;
  }
  .map {
    margin-top: 20px;
  }
  </style>
  