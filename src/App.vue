<script>
import Typed from 'typed.js';
import OneCard from './components/OneCard.vue'
export default {
	components:{OneCard},
	data() {
		return {
			awesome: true,
			page: true,
			heads: true,
			tel: "index"
		};
	},
	methods: {
		checced() {
			if (document.querySelector('input').checked) {
				document.querySelector('.block-of-menu').style = 'display:flex;'
			}
			else {
				document.querySelector('.block-of-menu').style = 'display:none;'
			}
		},
		setpage(){
			document.querySelector('.first-page').classList.add('scale-up-hor-left')
		}
	},
	mounted() {
		this.typed = new Typed('.Third', {
			strings: ['', 'Технологии, которые работают'],
			typeSpeed: 80,
		});

		this.typed = new Typed('.First', {
			strings: ['', 'АлгaРитм',],
			typeSpeed: 80,
		});
	}
};
</script>

<template>
	<div class="first-page"  v-if="page == true" >
		<div class="block-of-menu">
			<div class="rigth">
				<img src="/src/assets/logo.svg" alt="">
				<div class="but-block">
					<button @click="page = false">Наше ПО</button>
				</div>
			</div>
		</div>
		<header  v-if="heads == true">
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
				<button @click="page = false">Наше ПО</button>
			</div>
		</header>
		<div class="hams-line">
			<div class="hamburger">
				<input type="checkbox" name="" id="chekbox" @click="checced">
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
		<div class="telephons" id="third">
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
			<h6>© 2024 Все права защищены. Использование материалов сайта без согласия его авторов и активной ссылки на
				сайт
				– запрещено.</h6>
		</footer>
	</div>

	<div class="page-two scale-up-top" v-else @click="setpage()">
		<div class="head">
			<h1 @click="page = true">АлгаРитм</h1>
			<h3>Технологии, которые работают</h3>
		</div>
		<div class="block-search">
			<div class="block-of-text">
				<h1>
					Наше  предоставляемое <br>Програмное обеспечение
				</h1>
			</div>
			<div class="search">
				<input type="text">

				<svg width="90" height="85" viewBox="0 0 90 85" fill="none" xmlns="http://www.w3.org/2000/svg">
					<g clip-path="url(#clip0_29_230)">
						<path fill-rule="evenodd" clip-rule="evenodd"
							d="M39.2464 0.851562H0.900391V37.0672H20.6663C24.198 29.1757 30.891 22.8542 39.2464 19.5183V0.851562ZM0.900391 44.3103H18.4253C18.0983 46.1233 17.9276 47.9865 17.9276 49.8874C17.9276 63.5408 26.7188 75.2545 39.2464 80.2564V80.526H0.900391V44.3103ZM85.2615 37.0672H84.9788C79.6834 25.2345 67.2795 16.9311 52.8225 16.9311C50.8091 16.9311 48.8355 17.0922 46.9155 17.4014V0.851562H85.2615V37.0672ZM37.1006 49.887C37.1006 41.6866 44.1398 35.0386 52.8225 35.0386C61.5056 35.0386 68.5444 41.6866 68.5444 49.887C68.5444 58.0877 61.5056 64.7354 52.8225 64.7354C44.1398 64.7354 37.1006 58.0877 37.1006 49.887ZM52.8225 24.1741C37.7861 24.1741 25.5968 35.6863 25.5968 49.887C25.5968 64.0884 37.7861 75.6002 52.8225 75.6002C58.2593 75.6002 63.324 74.095 67.5746 71.5022L80.9663 84.1494L89.1004 76.4672L75.7088 63.8196C78.4545 59.8051 80.0483 55.0221 80.0483 49.887C80.0483 35.686 67.8589 24.1741 52.8225 24.1741Z"
							fill="black" />
					</g>
					<defs>
						<clipPath id="clip0_29_230">
							<rect width="90" height="85" fill="white" />
						</clipPath>
					</defs>
				</svg>

			</div>
		</div>
		<hr>
		<div class="cards-of-softs">
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
			<OneCard name ="Soft 1" count = 123></OneCard>
		</div>
	</div>
</template>

<style>
@import url("/src/assets/style.css");
@import url('/src/assets/media.css');
</style>
