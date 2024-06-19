<template>
    <section id="home">
      <div class="hero">
        <video autoplay muted loop class="background-video">
          <source src="@/assets/background-video.mp4" type="video/mp4">
        </video>
        <div class="hero-content">
          <h1>Интеллектуальные приложения: Будущее бизнеса</h1>
          <p>Узнайте, как ИИ и машинное обучение трансформируют рабочие процессы</p>
          <button>Узнать больше</button>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {}
  </script>
  
  <style>
  .hero {
    position: relative;
    height: 100vh;
    color: #fff;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .background-video {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
  }
  .hero-content {
    z-index: 1;
  }
  .hero h1 {
    font-size: 4em;
  }
  .hero p {
    font-size: 1.5em;
  }
  .hero button {
    padding: 10px 20px;
    font-size: 1em;
    cursor: pointer;
  }
  </style>
  