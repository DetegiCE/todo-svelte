<script>
	import Input from "./components/Input.svelte";
	import Todos from "./components/Todos.svelte";

	let todoList = [
		{
			id: 1,
			text: "WACCA",
			completed: false
		},
		{
			id: 2,
			text: "maimai",
			completed: false
		},
		{
			id: 3,
			text: "CHUNITHM",
			completed: true
		}
	];
</script>

<main>
	<div>
		<p>To Do List</p>
		<Input/>
		<Todos {todoList}/>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
