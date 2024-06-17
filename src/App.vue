<script>
export default {
  data() {
    return {
      awesome: true,
      page: true
    };
  },
  methods: {}
};
</script>

<template>
	<header v-if="page == true">
		<div class="but-block">
			<button>О нас</button>
		</div>
		<div class="but-block">
			<button>Где мы</button>
		</div>
		<img src="/src/assets/logo.svg" alt="" width="100px;" height="100px" />
		<div class="but-block">
			<button>Связь с нами</button>
		</div>
		<div class="but-block">
			<button>Наше ПО</button>
		</div>
	</header>
</template>

<style>
@import url("/src/assets/style.css");
</style>
