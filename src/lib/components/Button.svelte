<script>
	export let src;
</script>

<a href={src}>
	<slot />
</a>

<style>
	a {
		font-family: 'liberation-sans', sans-serif;
		font-size: 20px;
		border: none;
		background-color: #01bfaf;
		border-radius: 5px;
		padding: 8px 16px;
		width: fit-content;
		color: var(--text-color);
		text-decoration: none;
		transition: all 0.2s ease-in-out;
		cursor: pointer;
	}
</style>
