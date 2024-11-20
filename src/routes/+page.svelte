<script>
    import Cart from './../lib/components/Cart.svelte';
    import Button from '$lib/components/Button.svelte';
</script>

<h1>Welcome to SvelteKit</h1>

<!-- Komponenta Button -->
<Button color="red">Login</Button>

<!-- Komponenta Cart -->
<Cart 
    href="/example" 
    color="blue" 
    title="Okno" 
    content="Toto je okno. Mooooc hezký okno. Moc dobrý okno. Děkuji.">
    <!-- Dětský obsah pro kartu -->
    <Button color="green">Klikni hajzle</Button>
</Cart>
