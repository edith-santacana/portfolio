<template>
	<div class="banner-container">
		<div class="title">
			<div class="text">Hi!</div>
		</div>
		<background class="background"></background>
	</div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Background from './Background.vue';

@Options({
	components: { Background },
	props: {},
})
export default class Banner extends Vue {}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.banner-container {
	position: relative;
	background: blue;
	height: 100%;
	width: 100%;
}

.background {
	position: absolute;
	height: 100%;
	width: 100%;
}

.title {
	color: white;
	position: absolute;
	height: 100%;
	width: 100%;
	z-index: 2;
	display: flex;
}

.text {
	justify-content: center;
	margin: auto;
	font-weight: 700;
	font-size: 4em;
	text-shadow: rgb(202 66 66 / 79%) 6px 4px 11px;
}
</style>
