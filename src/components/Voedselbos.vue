<template>
  <div class="Voedselbos">
    <section class="info-text">
    <h1>Voudselbos</h1>
    <br/>
    <p>Lorem Ipsum is simply dummy text of the printing and typesetting industry.
      Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
      when an unknown printer took a galley of type and scrambled it to make a type specimen book.
      It has survived not only five centuries, but also the leap into electronic typesetting,
      remaining essentially unchanged.
      It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum
      passages, and more recently with desktop publishing software like Aldus PageMaker including
      versions of Lorem Ipsum.
    </p>
    </section>
    <br/>
    <div class="videos-voedselbos">
      <iframe class="voedselbos-items" src='https://www.youtube.com/embed//BSDwXIe-U6Q' frameborder='0' allowfullscreen></iframe>
      <iframe class="voedselbos-items" src='https://www.youtube.com/embed/fQ2udqitScM' frameborder='0' allowfullscreen></iframe>
      <iframe class="voedselbos-items" src='https://www.youtube.com/embed//BSDwXIe-U6Q' frameborder='0' allowfullscreen></iframe>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Voedselbos',
};
</script>

<style scoped>
  .Voedselbos{
    padding: 10px;
  }
  .info-text {
    padding: 10vh 10vh 10vh;
  }
  .videos-voedselbos {
    display: flex;
    flex-direction: row;
    overflow: auto;
    width: 100%;
  }
  .voedselbos-items {
    margin: 10px;
  }
</style>
