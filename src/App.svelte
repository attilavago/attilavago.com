<script>
	let name = 'world';
</script>

<style>
	body {
		padding: 0 !important;
		border: 0;
	}
	main {
		position: relative;
		display: grid;
		justify-items: center;
	}
	h1 {
		position: absolute;
		display: grid;
		align-self: center;
		text-align: center;
		background: rgba(127, 255, 212, 1);
    	padding: 20px;
    	border: solid 20px white;
	}
	.background {
		width: 0;
		height: 0;
		border-style: solid;
		border-width: 100vh 100vw 0 0;
		border-color: black transparent transparent transparent;
	}
</style>

<main>
<div class="background"></div>
<h1>life isn't binary, it's hexadecimal</h1>
</main>