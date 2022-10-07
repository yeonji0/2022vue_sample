<template>
  <div class="container">
    <ul class="d_Icon">
       <li v-for="item in data" :key="item">
        <a :href="item.href">
            <img :src="`img/directs/${item.src}`" alt="">
            <div class="txt">
                {{item.name}}
            </div>
        </a>
       </li>
    </ul>
  </div>
</template>

<script>


export default {
    props:["data"],
    data(){
        return{
            
        }
    }
}
</script>

<style lang="scss">
.d_Icon{
    display: flex;
    gap: 20px;
    img{width: 100px;}
    .txt{text-align: center;}

}

</style>