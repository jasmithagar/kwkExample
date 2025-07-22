<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
</script>

<div>
    <ArticleText>Now let's see how this pans out with median net worth.</ArticleText>
    <div>
        <Scroller layout="left">
            {#snippet sticky()}
            <img class="graph"src="blackwomangraph.png" alt="graph showing a black woman's median net worth" />
            {/snippet}

            {#snippet scrolly()}
                <ArticleText> Hmmm it's a bit hard to see, let's zoom in. </ArticleText>
                <!-- <ArticleText> let's zoom in</ArticleText> -->
            {/snippet}
        </Scroller>

        <Scroller layout="left">
            {#snippet sticky()}
            <img class="graph"src="bwzoom.png" alt="graph showing a Black female's median net worth" />
            {/snippet}

            {#snippet scrolly()}
                <ArticleText>Now it's better!</ArticleText>
                <ArticleText>The highlighted line is of a Black female's net worth.</ArticleText>
                <ArticleText>You can see that throughout the years it's has very low slope and the value is only at $14,020 in 2022.</ArticleText>
            {/snippet}
        </Scroller>
        <ArticleText>Now let's compare it to a White male's median net worth!</ArticleText>
        <Scroller layout="left">
            {#snippet sticky()}
            <img class="graph"src="wmzoom.png" alt="graph showing a White male's median net worth" />
            {/snippet}

            {#snippet scrolly()}
                <ArticleText>Wow, that looks <strong>very</strong> different from the graph we just saw.</ArticleText>
                <ArticleText>Even their low point in the 2008 recession doesn't compare to $14,020. It's almost 25 times as much as Black female's median net worth.</ArticleText>
                <ArticleText>Now do you really understand the value of those cents that Black females aren't even getting in the first place?</ArticleText>
                {/snippet}
        </Scroller>
    </div> 

    <ArticleText>There are also many other factors that play into this such as historical disadvantages, 
        limited access to financial services, housing inequites, the legal system, and I could go on and on and on. Today I 
        just wanted to show one element and really help you understand the wide disparity.
    </ArticleText>

    <ArticleText>
        The data I used for the median net worth is from 2023. It's 2025 and that gap isn't any smaller. 
    </ArticleText>

</div>

<style>
    .graph{
        width: 100%;
    }
</style>