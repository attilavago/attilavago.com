<script>
	let afterClickClass = '';
	let afterClickLayerClass = '';
	const afterClick = () => {
		afterClickClass = 'afterClickBackground';
		afterClickLayerClass = 'afterClickBackgroundLayer';
	}
</script>

<style>
	body {
		padding: 0 !important;
		border: 0;
	}
	main {
		position: relative;
		display: grid;
	}
	h1 {
		position: absolute;
		display: grid;
		align-self: center;
		justify-self: center;
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
		-webkit-transition: border-width 0.3s; /* Safari */
  		transition: border-width 0.3s;
	}
	.backgroundLayer {
		position: absolute;
		width: 0;
		height: 0;
		border-style: solid;
		border-width: 100vh 0 0 0;
		border-color: black transparent transparent black;
		-webkit-transition: border-width 0.3s; /* Safari */
		transition: border-width 0.3s;
		transition-delay: 0.3s;
	}
	.afterClickBackground {
		border-width: 100vh 20vw 0 0;
	}
	.afterClickBackgroundLayer {
		border-width: 100vh 0 0 20vw;
	}
</style>

<main>
<div class={"background " + afterClickClass}></div>
<div class={"backgroundLayer " + afterClickLayerClass}></div>
<h1 on:click={afterClick}>life isn't binary, it's hexadecimal</h1>
</main>