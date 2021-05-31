<template>
	<div id="app">
		<comp-header v-bind:title="title"/>
		<list-user v-bind:listUser="listUser"/>
		<comp-footer />
	</div>
</template>

<script>
import CompHeader from './components/CompHeader.vue';
import CompFooter from './components/CompFooter.vue';
import ListUser from './components/ListUser.vue';
export default {
	name: 'app',
	data () {
		return {
			msg: 'Hello VueJs',
			title: 'Hello VueJs - Header....',
			listUser: [
				{id: 100, email: '1@gmail.com', activate: true},
				{id: 101, email: '2@gmail.com', activate: false},
				{id: 102, email: '3@gmail.com', activate: true},
				{id: 103, email: '4@gmail.com', activate: true},
				{id: 104, email: '5@gmail.com', activate: false},
				{id: 105, email: '6@gmail.com', activate: false},
				{id: 106, email: '7@gmail.com', activate: false},
				{id: 107, email: '8@gmail.com', activate: false}
			]
		}
	},
	components: {
		CompHeader,
		CompFooter,
		ListUser
	}
}
</script>

<style>
	#app {
		font-family: 'Avenir', Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}

	h1, h2 {
		font-weight: normal;
	}

	ul {
		list-style-type: none;
		padding: 0;
	}

	li {
		display: inline-block;
		margin: 0 10px;
	}

	a {
		color: #42b983;
	}
</style>
