<script>
export default {
	name: "Nav",
	props: [],
	store: [],
	components: {},

	mounted() {},

	data() {
		return {};
	},

	methods: {
		sortFloor(floor) {
			console.log(floor);
		},
	},

	watch: {},
};
</script>

<template>
	<div class="nav">
		<div class="nav__div" @click="sortFloor(1)">1st Floor</div>
		<div class="nav__div" @click="sortFloor(2)">2nd Floor</div>
		<div class="nav__div" @click="sortFloor(3)">3rd Floor</div>
		<div class="nav__div" @click="sortFloor(4)">4th Floor</div>
	</div>
</template>

<style lang="scss" scoped>
.nav {
	display: flex;
	justify-content: center;
	align-items: center;
	align-self: center;
	max-height: 10vh;
	border-radius: 1rem;
	padding: 0.3rem;
	margin-bottom: 1vh;

	&__div {
		margin: 0.5rem;
	}
}
</style>
