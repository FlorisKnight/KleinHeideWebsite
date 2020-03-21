<template>
    <div class="FooterComp">
      <img class="logo-footer" src="../assets/img/Frog.png"/>
      <p>Klein Heide &#9400; 2020</p>
    </div>
</template>

<script>
export default {
  name: 'FooterComp',
};
</script>

<style scoped>
  .FooterComp {
    width: 100%;
    background-color: #0d2c20;
    display: flex;
    justify-content: center;
    flex-direction: column;
    padding: 5vh;
  }
  .logo-footer {
    height: 100px;
    background-image: linear-gradient(
      120deg,
      rgba(212, 252, 121, 1) 0%,
      rgba(150, 230, 161, 1) 100%);
    border-radius: 100%;
    align-self: center;
  }
  p {
    color: #eeeeee;
    align-self: center;
  }
</style>
