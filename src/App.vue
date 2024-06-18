<script>
export default {
  data() {
    return {
      awesome: true,
      page: false,
	  heads: true
    };
  },
  methods: {}
};
</script>

<template v-if="page == true">
	<header v-if="heads == true">
		<div class="but-block">
			<button>О нас</button>
		</div>
		<div class="but-block">
			<button>Где мы</button>
		</div>
		<img src="/src/assets/logo.svg" alt="" width="100%;" height="100px" />
		<div class="but-block">
			<button>Связь с нами</button>
		</div>
		<div class="but-block">
			<button>Наше ПО</button>
		</div>
	</header>
	<div class="block-start">
		<div class="texts">
		<h1 class="First">АлгаРитм</h1>
		<h3 class="Third">Технологии, которые работают</h3>
		</div>
		<img src="/src/assets/ноуты1.jpg" alt="ноутбуки" >
	</div>
	<hr>
	<div class="block-about">
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>А также стремящиеся вытеснить традиционное производство,
				 нанотехнологии преданы социально-демократической анафеме.
				  Разнообразный и богатый опыт говорит нам,
				 что постоянное информационно-пропагандистское.</h6>
		</div>
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>А также стремящиеся вытеснить традиционное производство,
				 нанотехнологии преданы социально-демократической анафеме.
				  Разнообразный и богатый опыт говорит нам,
				 что постоянное информационно-пропагандистское.</h6>
		</div>
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>А также стремящиеся вытеснить традиционное производство,
				 нанотехнологии преданы социально-демократической анафеме.
				  Разнообразный и богатый опыт говорит нам,
				 что постоянное информационно-пропагандистское.</h6>
		</div>
	</div>
	<hr>
	<div class="info-map">
		<h1>Где нас найти?</h1>
		<br>
		<div class="map"></div>
	</div>


	<footer></footer>
</template>

<style>
@import url("/src/assets/style.css");
</style>
