<script>
    let { children } = $props();
</script>

<div class="article-text">
    <p>
        {@render children()}
    </p>
</div>

<style>
    .article-text {
        margin: 50vh auto;
        width: 50%;
        background-color: #E6A84E;
        color: #FAF8D4; 
        border: solid #793F37 3px;
        border-radius: 20px;
        padding: 20px;
        box-shadow: 16px 16px #8aa6df;
    }
</style>
