<script>
    let { href = "#", color = "default", children, title = "Default Title", content = "Default content" } = $props();

    let Cart_class = `${color} cart`;
</script>

<style>
    .cart {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: flex-start;
        background-color: #f9f9f9;
        border: 2px solid #ccc;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        padding: 16px;
        width: 300px;
        max-width: 100%;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        margin-top: 20px;
    }
    .cart:hover {
        transform: translateY(-5px);
        box-shadow: 0 6px 12px rgba(0, 0, 0, 0.2);
    }
    h1 { font-size: 1.5rem; margin: 0 0 8px 0; color: #333; }
    p { font-size: 1rem; color: #555; margin: 0 0 16px 0; }
    .children { margin-top: 16px; width: 100%; }
</style>

<div class={Cart_class}>
    <div>
        <h1>{title}</h1>
        <p>{content}</p>
    </div>
    <div class="children">
        {@render children()}
    </div>
</div>
