<template>
  <section class="service">
    <div class="section__container service__container">
      <p class="section__subtitle">What I Offer!</p>

      <h2 class="section__title"><span>My</span> Services</h2>

      <div class="service__grid">
        <div class="service__card">
          <i class="fas fa-mobile-alt"></i>
          <h4>Web Design</h4>
          <p>
            We are dedicated to providing high-quality web design services that
            are tailored to meet the specific needs of our clients.
          </p>
          <a href="#" class="read__more">Read more...</a>
        </div>

        <div class="service__card">
          <i class="fas fa-code"></i>
          <h4>Web Development</h4>
          <p>
            We use the latest web technologies and development tools to create
            websites that are fast, secure, and scalable.
          </p>
          <a href="#" class="read__more">Read more...</a>
        </div>

        <div class="service__card">
          <i class="fas fa-palette"></i>
          <h4>Creative Design</h4>
          <p>
            Our approach is collaborative, and we encourage your feedback
            throughout the design process to ensure that we are meeting your
            expectations.
          </p>
          <a href="#" class="read__more">Read more...</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.service,
footer {
  background-color: var(--primary-color);
}
.service__grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
  margin-top: 5rem;
}
.service__card {
  display: grid;
  align-items: flex-start;
  gap: 1rem;
  padding: 2rem;
  background-color: var(--text-dark);
  border-radius: 5px;
}
.service__card i {
  font-size: 1.5rem;
}
.service__card h4 {
  font-size: 1.2rem;
  font-weight: 500;
}
.service__card p {
  color: var(--text-light);
}
.service__card .read__more {
  width: max-content;
  padding: 0.5rem 1rem;
  color: var(--text-light);
  font-size: 0.8rem;
  border-radius: 5px;
  background-color: rgba(255, 255, 255, 0.05);
  cursor: pointer;
}

@media (max-width: 888px) {
  .service__grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 1rem;
    margin-top: 5rem;
  }
}
@media (max-width: 640px) {
  .service__grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 1rem;
    margin-top: 5rem;
  }
}
</style>
