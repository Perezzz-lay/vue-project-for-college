<script>
export default{
props:{
    name:{
        type: String
    },
    count:{
        type: Number
    }
}
}
</script>

<template>
<div class="card">
    <div class="about-logo">
        <img src="" alt="">
        <h1>{{name}}</h1>
    </div>
    <div class="downloads">
        <img src='' alt="">
        <h5>{{count}}</h5>
    </div>
    <div class="rating">
        <div class="stars"></div>
        <button>Подробнее</button>
    </div>
</div>
</template>

<style>

</style>