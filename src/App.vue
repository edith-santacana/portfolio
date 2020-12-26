<template>
	<Banner class="full-screen" />
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Banner from './components/Banner.vue';

@Options({
	components: {
		Banner,
	},
})
export default class App extends Vue {}
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
  height: 100%;
	width: 100%;
}

html,
body {
	height: 100vh;
	width: 100vw;
  margin: 0;
  padding: 0;
}

.full-screen {
	height: 100%;
	width: 100%;
}
</style>
