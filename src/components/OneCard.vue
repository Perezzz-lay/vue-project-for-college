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
        <img src="/src/assets/network-svgrepo-com.svg" alt="">
        <h1>{{name}}</h1>
    </div>
    <div class="downloads">
        <img src='' alt="">
        <h5>{{count}}</h5>
    </div>
    <div class="rating">
        <div class="stars">
            <img src="/src/assets/star-svgrepo-com.svg" alt="" width="20px">
            <img src="/src/assets/star-svgrepo-com.svg" alt="" width="20px">
            <img src="/src/assets/star-svgrepo-com.svg" alt="" width="20px">
            <img src="/src/assets/star-svgrepo-com.svg" alt="" width="20px">
            <img src="/src/assets/star-svgrepo-com.svg" alt="" width="20px">
        </div>
        <button>Подробнее</button>
    </div>
</div>
</template>

<style>
.card{
    width: 300px;
    height: 300px;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    align-content: flex-start;
    justify-content: center;
    align-items: center;
}
.card:hover{
    -webkit-animation: scale-down-center 0.4s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
	        animation: scale-down-center 0.4s cubic-bezier(0.250, 0.460, 0.450, 0.940) both;
}
.about-logo{
    img{
        width: 100px;
        height: 100px;
    }
}
.rating{
      display: flex;
      flex-direction: row;
      flex-wrap: nowrap;
      justify-content: space-around;
      align-items: center;
      width: 100%;

      button{
        background-color: black;
        color: white;
        width: 124px;
        border-radius: 50px;
        text-align: center;
        font-family: 'Font3';
        font-size: 115%;
      }
    }
    @-webkit-keyframes scale-down-center {
  0% {
    -webkit-transform: scale(1);
            transform: scale(1);
  }
  100% {
    -webkit-transform: scale(0.9);
            transform: scale(0.9);
  }
}
@keyframes scale-down-center {
  0% {
    -webkit-transform: scale(1);
            transform: scale(1);
  }
  100% {
    -webkit-transform: scale(0.9);
            transform: scale(0.9);
  }
}
@media screen and (max-width: 600px){
    .card{
    width: 200px;
    height: 200px;
    display: flex;
    flex-direction: column;
    flex-wrap: nowrap;
    align-content: flex-start;
    justify-content: center;
    align-items: center;
}
.about-logo{
    img{
        margin-top: 1vh;
        width: 60px;
        height: 60%;
    }
    h1{
        font-size: 20px;
    }
}
.rating{
      display: flex;
      flex-direction: row;
      flex-wrap: nowrap;
      justify-content: space-around;
      align-items: center;
      width: 80%;
.stars{
    display: none;
}
      button{
        background-color: black;
        color: white;
        width: 124px;
        border-radius: 50px;
        text-align: center;
        font-family: 'Font3';
        font-size: 115%;
      }
    }
}
</style>