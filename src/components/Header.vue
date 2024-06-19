<template>
    <header>
      <nav>
        <ul>
          <li><a href="#home">Главная</a></li>
          <li><a href="#about">О Приложениях</a></li>
          <li><a href="#benefits">Преимущества</a></li>
          <li><a href="#examples">Примеры</a></li>
          <li><a href="#contact">Контакты</a></li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script>
  export default {}
  </script>
  
  <style>
  header {
    background: #333;
    color: #fff;
    padding: 10px 0;
  }
  nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
  }
  nav ul li {
    margin: 0 15px;
  }
  nav ul li a {
    color: #fff;
    text-decoration: none;
  }
  </style>
  