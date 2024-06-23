<script>
import Typed from 'typed.js';

export default {
	data() {
		return {
			awesome: true,
			page: false,
			heads: true
		};
	},
	methods: {
	checced(){
		if(document.querySelector('input').checked){
			document.querySelector('.block-of-menu').style = 'display:flex;'
		}
		else{
			document.querySelector('.block-of-menu').style = 'display:none;'
		}
	}
	},
	mounted(){
		this.typed = new Typed('.Third', {
         strings: ['','Технологии, которые работают'],
         typeSpeed: 80,
      });

		this.typed = new Typed('.First', {
         strings: ['','АлгaРитм',],
         typeSpeed: 80,
      });

	}
};
</script>

<template v-if="page == true">
<div class="block-of-menu">
	<div class="rigth">
		<img src="/src/assets/logo.svg" alt="">
		<div class="but-block">
			<button>Наше ПО</button>
		</div>
</div>
</div>
	<header v-if="heads == true">
			<div class="but-block">
			<a href="#first"><button>О нас</button></a>
		</div>
		<div class="but-block">
			<a href="#second"><button>Где мы</button></a>
		</div>
		<div style=" height: 100px"></div>
		<div class="but-block">
			<a href="#third"><button>Связь с нами</button></a>
		</div>
		<div class="but-block">
			<a href=""><button>Наше ПО</button></a>
		</div>
	</header>
	<div class="hams-line">
		<div class="hamburger">
		<input type="checkbox" name="" id="" @click="checced">
		<div class="ham-line">&nbsp;</div>
		<div class="ham-line">&nbsp;</div>
		<div class="ham-line">&nbsp;</div>
	</div>
	</div>
	<div class="block-start">
		<div class="texts">
			<h1 class="First">АлгаРитм</h1>
			<h3 class="Third">Технологии, которые работают</h3>
		</div>
		<img src="/src/assets/ноуты1.jpg" alt="ноутбуки" />
	</div>
	<hr />
	<div class="block-about" id="first">
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
	<div class="info-map" id="second">
		<h1>Где нас найти?</h1>
		<br />
		<div class="map" id="map">
			<iframe class="maps"
				src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1112.9968703680577!2d54.23494878632456!3d56.08802498437215!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x43e0a1130e73c9c5%3A0x8200de995e685b50!2z0JDQm9CT0JDRgNC40YLQvA!5e0!3m2!1sru!2sru!4v1718732879387!5m2!1sru!2sru"
				style="border: 0" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
			</iframe>
		</div>
	</div>
	<hr>
	<div class="telephons" id="third" >
		<h1>Связаться с нами</h1>
		<div class="more-tels">
			<div class="telphone">
				<h3>Телефон 1</h3>
				<h4>+7 (999) 999-99-99</h4>
			</div>
			<div class="telphone">
				<h3>Телефон 1</h3>
				<h4>+7 (999) 999-99-99</h4>
			</div>
			<div class="telphone">
				<h3>Телефон 1</h3>
				<h4>+7 (999) 999-99-99</h4>
			</div>
		</div>
	</div>
	<footer>
		<h5>ООО <ИнфоСофтСервис>
		</h5>
		<h6>© 2024 Все права защищены. Использование материалов сайта без согласия его авторов и активной ссылки на сайт
			– запрещено.</h6>
	</footer>
</template>

<style>

@import url("/src/assets/style.css");
@import url('/src/assets/media.css');
</style>
