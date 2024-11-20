<script>
    // Získání atributů z `$props`, s výchozími hodnotami
    let { href = "#", color = "default", children } = $props();

    // Dynamická třída
    let Button_class = `${color} button`;
</script>

<a {href} class={Button_class}>
    {@render children()} <!-- Správné použití {@render} pro vykreslení children -->
</a>

<style lang="scss">
    /* Stylování tlačítka */
    .button {
        padding: 10px 20px;
        border-radius: 5px;
        text-decoration: none;
        display: inline-block;
    }
    .default {
        background-color: #ccc;
        color: #000;
    }
    .red {
        background-color: #fc0000;
        color: #ffffff;
    }
</style>
