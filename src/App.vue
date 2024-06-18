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
		<img src="/src/assets/ноуты1.jpg" alt="ноутбуки" />
	</div>
	<hr />
	<div class="block-about">
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>
				А также стремящиеся вытеснить традиционное производство, нанотехнологии
				преданы социально-демократической анафеме. Разнообразный и богатый опыт
				говорит нам, что постоянное информационно-пропагандистское.
			</h6>
		</div>
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>
				А также стремящиеся вытеснить традиционное производство, нанотехнологии
				преданы социально-демократической анафеме. Разнообразный и богатый опыт
				говорит нам, что постоянное информационно-пропагандистское.
			</h6>
		</div>
		<div class="about">
			<h1>Кто мы?</h1>
			<h6>
				А также стремящиеся вытеснить традиционное производство, нанотехнологии
				преданы социально-демократической анафеме. Разнообразный и богатый опыт
				говорит нам, что постоянное информационно-пропагандистское.
			</h6>
		</div>
	</div>
	<hr />
	<div class="info-map">
		<h1>Где нас найти?</h1>
		<br />
		<div class="map" id="map">
			<iframe class="maps"
				src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1112.9968703680577!2d54.23494878632456!3d56.08802498437215!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x43e0a1130e73c9c5%3A0x8200de995e685b50!2z0JDQm9CT0JDRgNC40YLQvA!5e0!3m2!1sru!2sru!4v1718732879387!5m2!1sru!2sru"
				style="border: 0" allowfullscreen="" loading="lazy"
				referrerpolicy="no-referrer-when-downgrade"></iframe>
		</div>
	</div>
	<hr>
	<div class="telephons">
		<h1></h1>
		<div class="more-tels">
			<h4></h4>
			<h4></h4>
			<h4></h4>
		</div>
	</div>
	<footer></footer>
</template>

<style>
@import url("/src/assets/style.css");
</style>
