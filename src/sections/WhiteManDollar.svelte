<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
</script>



<div class="text">
    <ArticleText>Let's <strong>visualize</strong> this!</ArticleText>
    <div>
        <Scroller layout="right">
            {#snippet sticky()}
                <!-- <img class="duck-img" src="duck.png" alt="KWK rubber duck!" /> -->
                <img class="dollar-img" src="dollar.png" alt="green bill with 100 circles" />
            {/snippet}
            {#snippet scrolly()}
                <!-- <img class="duck-img" src="duck.png" alt="KWK rubber duck!" /> -->
                <ArticleText>Here's a dollar! Now imagine you're a white man and you made this full dollar at work! Amazing right?</ArticleText>
            {/snippet}
        </Scroller>
    </div>
    
</div>

<style>
    :global(body){
        background-color: #FFD95C;
    }
    .dollar-img{
         width: 100%;
        margin: 0px auto;
    }
    
</style>