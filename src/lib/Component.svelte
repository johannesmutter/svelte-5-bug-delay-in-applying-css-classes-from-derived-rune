<script>
	let {
		rows = 3
	} = $props();
  const title_font = $derived( rows <= 3 ? 'text-system' : 'text-intro' );
</script>

<p class='{title_font} title bold'>Dynamic class added at start: This text will be NOT bold initially</p>
<p class='title bold {title_font} '>Dynamic class added at ed: This text will be bold initially</p>


<style>
	.bold {
		font-weight: 700 !important;
	}
	.text-system {
		font-size: 1rem;
		font-weight: 400;
	}
	.text-intro {
		font-size: 3rem;
		font-weight: 400;
	}
</style>