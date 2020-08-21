<template>
  <div class="container">
    <div class="row mb-5">
      <div class="col-lg-6 d-flex align-items-center justify-content-center flex-column text-left">
        <div class="title app-name">Цифровой<br> искусствовед</div>
      </div>
      <div class="col-lg-3 d-flex align-items-center justify-content-center flex-column">
        <div class="title">IXX?</div>
        <div class="title">XXI?</div>
      </div>
      <div class="col-lg-3">
        <img src="/static/icon.png">
      </div>
    </div>
    <vue-dropzone ref="myVueDropzone" id="dropzone" :options="dropzoneOptions"></vue-dropzone>
  </div>
</template>

<script>
  import vue2Dropzone from 'vue2-dropzone'
  import 'vue2-dropzone/dist/vue2Dropzone.min.css'

  export default {
    name: 'Main',
    components: {
      vueDropzone: vue2Dropzone
    },
    data () {
      return {
      }
    },
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  @font-face {
    font-family: "BreeSerif";
    src: local("BreeSerif"),
    url(/fonts/BreeSerif-Regular.ttf) format("truetype");
  }
  h1, h2 {
    font-weight: normal;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }
  li {
    display: inline-block;
    margin: 0 10px;
  }
  a {
    color: #42b983;
  }
  .vue-dropzone {
    border: 2px dashed #e5e5e5;
  }
  .title {
    font-family: "BreeSerif";
    font-weight: bold;
    font-size: 50px;
    line-height: 50px;
    color: #a66403
  }
  .title:nth-child(2) {
    margin-left: 120px;
  }
  .title.app-name {
    font-size: 80px;
    line-height: 80px;
  }
</style>
