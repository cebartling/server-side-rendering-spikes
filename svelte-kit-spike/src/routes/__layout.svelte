<script lang='ts'>
	import '../app.css';
	import Header from '$lib/header/Header.svelte';
	import Footer from '$lib/footer/Footer.svelte';
</script>

<div class='container py-3'>
	<Header />
	<main>
		<slot />
	</main>
	<Footer />
</div>

<style>
    @media (min-width: 768px) {
        .bd-placeholder-img-lg {
            font-size: 3.5rem;
        }
    }

    .container {
        max-width: 960px;
    }
</style>
