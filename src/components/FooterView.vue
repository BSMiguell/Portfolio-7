<template>
  <footer>
    <div class="section__container footer__container">
      <div class="footer__content">
        <h2 class="section__title">Contact <span>Me!</span></h2>

        <p class="section__subtitle">If you have any project in your mind</p>

        <div class="footer__details">
          <p>
            You can reach me through the contact form provided on this website.
            Simply fill out the form with your name, email address, and message,
            and I will get back to you as soon as possible.
          </p>

          <p>Digital Agency Network, 20</p>
          <p>Eastbourne Terrace, London W2 6LG,</p>
          <p>United Kingdom</p>
        </div>

        <div class="social__icons">
          <a href="#" class="icon"> <i class="fab fa-facebook"></i></a>
          <a href="#" class="icon"><i class="fas fa-envelope"></i></a>
          <a href="#" class="icon"><i class="fab fa-twitter"></i></a>
          <a href="#" class="icon"><i class="fab fa-linkedin"></i></a>
        </div>
      </div>

      <form class="footer__form">
        <input type="text" placeholder="Your Name" />
        <input type="text" placeholder="Your Email Address" />
        <input type="text" placeholder="Your Phone Number" />
        <textarea cols="30" rows="10" placeholder="Your Idea"></textarea>
        <button type="submit" class="btn">Send Message</button>
      </form>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style>
.footer__container {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 2rem;
}
.footer__content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
}
.footer__details {
  font-size: 0.8rem;
  color: var(--text-light);
  margin: 2rem 0;
  display: grid;
  gap: 1rem;
}
.social__icons {
  display: flex;
  align-items: center;
  gap: 1rem;
}
.social__icons .icon {
  padding: 0.5rem 0.8rem;
  border-radius: 5px;
  color: var(--white);
  background-color: var(--secondary-color);
  transition: 0.3s;
  cursor: pointer;
}
.social__icons .icon:hover {
  background-color: var(--secondary-color-dark);
}
.footer__form {
  display: grid;
  gap: 1rem;
}
.footer__form :is(input, textarea) {
  padding: 1rem;
  background-color: var(--text-dark);
  outline: none;
  border: none;
  border-radius: 5px;
  color: var(--white);
}
.footer__form textarea {
  resize: none;
  font-family: "Poppins", sans-serif;
}
.footer__form button {
  width: max-content;
}
@media (max-width: 888px) {
  .footer__container {
    grid-template-columns: repeat(1, 1fr);
  }
}
</style>
