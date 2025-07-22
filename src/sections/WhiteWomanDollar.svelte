<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
    let visible = true;

    function ToggleVisibility(){
        visible = !visible;
    }
</script>


<div>
    <Scroller layout="right">
        {#snippet sticky()}
        <button on:click={ToggleVisibility} class="button">
            {#if visible}
                <img class="dollar" src="dollar.png" alt="green bill with 100 circles" />
            {:else}
                <img class="dollar" src="white-woman-dollar.png" alt="green bill with 100 circles 79 filled in black" />
            {/if}

        </button>
        {#if visible}
            <h2> White Man Dollar </h2>
        {/if}

        {#if !visible}
            <h2> White Woman Dollar </h2>
        {/if}
        {/snippet}
        {#snippet scrolly()}
            <ArticleText>Now you're a white woman, click on the <strong>dollar</strong> to see how much of the 100 cents you get to take home!</ArticleText>
            <ArticleText>Yup what you saw was right! You only made <strong>79.6 cents</strong> of the dollar.</ArticleText>
        {/snippet}
    </Scroller>
    <ArticleText>Here's what that looks for a <strong> Black Woman </strong> in the United States.</ArticleText>

</div>

<style>
    .dollar{
        width: 100%;
        margin: 0px auto;
    }
    .button{
        background: none;
        border: none;
        padding: 0;
        cursor: pointer;
        height: 300px;
    }
    
</style>