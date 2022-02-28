<template>
    <section>
       <!-- <img src="../assets/img/jumbo-bg.png" alt=""> -->
       <img :src="require('../assets/img/' + imgName)" alt="">
       <div class="banner_text">
           <h2>Sono il testo del Banner</h2>
       </div>
    </section>
</template>

<script>
export default {
  name: "Banner",
  data: function() {
      return {
          imgName: "jumbo-bg.png"
      }
  }
};
</script>

<style scoped>
section {
    margin: 30px 0;
    widows: 100%;
    position: relative;
}
img {
    width: 100%;
}
.banner_text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 50px;
    color: yellow;
}

</style>