<template>
  <div class="hello">
    <div>
        <img src="" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">卡片三</h5>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {};
  },
  created(){
    console.log(this.$route.params.id);
    this.$http.get('https://randomuser.me/api/').then((response) => {
        console.log(response);
    })
  },
}
</script>