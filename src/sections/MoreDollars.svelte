<script>
    import Scroller from "../lib/Scroller.svelte";
    import ArticleText from "../lib/ArticleText.svelte";
    let visible = true;

    function ToggleVisibility(){
        visible = !visible;
    }
</script>


<div>
        <h2 class="text">Remember this is what the white man in the United States gets:</h2>
        <img class="dollar" src="dollar.png" alt="green bill with 100 circles" />
        <h2 class="text">Now this is what a Black Woman gets out of the dollar</h2>
        <img class="dollar" src="black-woman-dollar.png" alt="green bill with 100 circles 66 filled in black" />
        <div class="removemargins">
            <p class="ptext">Wow, now you're only get 66.5 cents of the dollar.</p>
        </div>
        
</div>

<style>
    .text{
        display:flex;
        justify-content: center;
    }
    .dollar{
        display: block;
        width: 50%;
        margin: 0px auto;
    }

    .removemargins{
        display:flex;
        justify-content: center;
    }
    .ptext{
        width: 50%;
        background-color: #E6A84E;
        color: #FAF8D4; 
        border: solid #793F37 3px;
        border-radius: 20px;
        padding: 20px;
        box-shadow: 16px 16px #8aa6df;
    }
    
</style>