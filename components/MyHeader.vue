<template>
  <header class="header-container">
    <h1>Liana</h1>
    <ul class="header-links">
      <li>Acceuil</li>
      <li>About</li>
    </ul>
  </header>
</template>

<script>
export default {};
</script>

<style>
.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #0f0f0f;
  color: #ffffff;
  padding: 10px 40px;

  width: 100%;
}

.header-links {
  display: flex;
  justify-content: end;
  gap: 20px;
}
</style>