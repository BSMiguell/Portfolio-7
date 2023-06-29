<template>
  <section class="project">
    <div class="section__container project__container">
      <p class="section__subtitle">Portfolio</p>

      <h2 class="section__title"><span>Latest</span> Project</h2>

      <div class="project__grid">
        <div class="project__card">
          <img src="../assets/project-1.png" alt="project" />
        </div>

        <div class="project__card">
          <img src="../assets/project-2.png" alt="project" />
        </div>

        <div class="project__card">
          <img src="../assets/project-3.png" alt="project" />
        </div>

        <div class="project__card">
          <img src="../assets/project-4.png" alt="project" />
        </div>

        <div class="project__card">
          <img src="../assets/project-5.png" alt="project" />
        </div>

        <div class="project__card">
          <img src="../assets/project-6.png" alt="project" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.project__grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
  margin-top: 5rem;
}
.project__card {
  display: grid;
  place-content: center;
  border-radius: 5px;
  overflow: hidden;
  cursor: pointer;
}
.project__card img {
  transition: scale 0.3s;
}
.project__card:hover img {
  scale: 1.1;
}

@media (max-width: 888px) {
  .project__grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
    margin-top: 5rem;
  }
}
@media (max-width: 640px) {
  .project__grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 1rem;
    margin-top: 5rem;
  }
}
</style>
