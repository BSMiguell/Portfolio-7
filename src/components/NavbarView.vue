<template>
  <div class="">
    <nav>
      <div class="nav__logo"><a href="#">BS<span>M</span>:D.</a></div>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style>
nav {
  position: absolute;
  width: 100%;
  top: 0;
  left: 50%;
  transform: translateX(-50%);
  max-width: var(--max-width);
  padding: 1rem;
}

nav .nav__logo a {
  font-size: 1.5rem;
  font-weight: 600;
}

nav .nav__logo a span {
  color: var(--secondary-color);
}
</style>
