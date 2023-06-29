<template>
  <section class="about">
    <div class="section__container about__container">
      <div class="about__image">
        <img src="../assets/about-bg.jpg" alt="about" />
      </div>

      <div class="about__content">
        <h2 class="section__title">About <span>Me</span></h2>
        <p class="section__subtitle">Vue/JS Web Developer.!</p>
        <p class="about__details">
          Welcome to my web developer portfolio! I'm BSM, a skilled and creative
          web developer with a passion for creating beautiful, responsive, and
          user-friendly websites. I've been working on various web projects,
          including personal blogs and e-commerce platforms, showcasing my
          expertise in Vue.js. I strive to deliver high-quality solutions that
          not only meet the client's requirements but also provide a seamless
          and enjoyable user experience. Feel free to explore my portfolio and
          witness my commitment to excellence in web development.
        </p>
        <button class="btn">More About</button>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.about,
.project {
  background-color: var(--text-dark);
}
.about__container {
  display: flex;
  flex-direction: row;
  gap: 1rem;
}

.about__image,
.about__content {
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.about__image img {
  max-width: 350px;
}
.about__details {
  padding: 2rem 0;
  color: var(--text-light);
  text-align: center;
}

@media (max-width: 888px) {
  .about__container {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
}
</style>
