<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
</script>

<div>
    <Scroller layout="right">
        {#snippet sticky()}
            <img class="duck-img" src="duck.png" alt="KWK rubber duck!" />
        {/snippet}

        {#snippet scrolly()}
            <ArticleText>
                Hey you!
            </ArticleText>
            <ArticleText>
                <strong>
                    Yeah YOU
                </strong>
            </ArticleText>
            <ArticleText>
                What do you know about the <strong>wealth gap?</strong>
            </ArticleText>
            <ArticleText>
                Oh you know about the huge disparities regarding race and gender?
            </ArticleText>
            <ArticleText>
                Well since you know everything, I guess we're done.
            </ArticleText>
            <ArticleText>
               Just kidding!
            </ArticleText>
        {/snippet}
    </Scroller>
</div>
