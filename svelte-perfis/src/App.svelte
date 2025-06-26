<script lang="ts">
	let name: string = 'João';
	let descricao = 'Esta é minha primeira aplicação Svelte!'
	let src = 'https://upload.wikimedia.org/wikipedia/pt/b/b4/Corinthians_simbolo.png';
	let alt = 'Imagem do Corinthians';
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>{descricao}</p>
	<img {src} {alt} height="300">
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