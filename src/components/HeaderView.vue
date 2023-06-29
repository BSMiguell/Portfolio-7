<template>
  <header>
    <div class="section__container header__container">
      <p><span>Hello</span> I'm</p>

      <h1>BSM</h1>

      <h2 class="section__title">Vue/JS <span>Web Developer.</span></h2>
      <p>
        Welcome to my web developer portfolio! I'm BSM, a skilled and creative
        web developer with a passion for creating beautiful, responsive, and
        user-friendly websites. I've been working on various web projects,
        including personal blogs and e-commerce platforms, showcasing my
        expertise in Vue.js. I strive to deliver high-quality solutions that not
        only meet the client's requirements but also provide a seamless and
        enjoyable user experience. Feel free to explore my portfolio and witness
        my commitment to excellence in web development.
      </p>

      <div class="action__btns">
        <button class="btn">Say Hello</button>

        <a href="#" class="video">
          <div class="play">
            <i class="fas fa-play"></i>
          </div>
          <span>Watch My Video</span>
        </a>
      </div>
    </div>
  </header>
</template>

<script>
export default {};
</script>

<style>
@import "~@fortawesome/fontawesome-free/css/all.css";

header {
  height: 100vh;
  background-image: url("../assets/header-bg.png");
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}

.header__container {
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}
.header__container p {
  color: var(--text-light);
  max-width: 400px;
  margin: 1rem 0;
}
.header__container p span {
  color: var(--white);
  padding: 0.5rem 1rem;
  background-color: var(--secondary-color);
  border-radius: 5px;
  margin-right: 1rem;
}
.header__container h1 {
  font-size: 3rem;
  line-height: 3rem;
}
.action__btns {
  display: flex;
  align-items: center;
  gap: 1rem;
  flex-wrap: wrap;
}

.action__btns .video {
  display: flex;
  align-items: center;
  gap: 1rem;
  cursor: pointer;
}

.action__btns .video .play {
  height: 50px;
  width: 50px;
  display: grid;
  place-content: center;
  font-size: 1.5rem;
  border-radius: 100%;
  background-color: var(--secondary-color);
  transition: 0.3s;
}

.action__btns .video span {
  font-size: 1rem;
  font-weight: 600;
}

.action__btns .video:hover .play {
  background-color: var(--secondary-color-dark);
}
</style>
