<script>

	let number = 0;
	function plus() {
		number++;
	}

	function minus() {
		number--;
	}

</script>

<main>
		
	<h1>Counter</h1>
	
	<div class="number">
		<p>{number}</p>
		<div>
			<button on:click={plus}>+</button>
			<button on:click={minus}>-</button>
			<button on:click={() => number=0}>Reset</button>
		</div>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 1080px;
		margin: 0 auto;
	}

	h1 {
		color: #ff1d58;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	.number {
		display: inline-block;
		text-align: center;
		border: 1px solid #f75990;
		width: 25rem;
	
	}

	.number p {
		color: #f75990;
		font-size: 200px;
	}
</style>