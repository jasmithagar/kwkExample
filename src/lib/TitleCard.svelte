<script>
    let { title, subtitle } = $props();
</script>

<!-- <div class="title-card">
    <div class="content">
        <h1>{title}</h1>
        <p>{subtitle}</p>
    </div>
</div> -->

<div class="outer">
    <div class="inner">
        <img class="img" src=dollar.png>
        <h1>{title}</h1>
        <p><mark>{subtitle}</mark></p>
    </div>
</div>


<style>

    .outer{
        display:flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .inner{
        display:flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

        h1 {
        font-size: 3rem;
        margin: 0;
        color: #793F37;
        text-shadow: 1px 1px 0 #F0F1F3;
        font-family: 'Verdana';
    }

    p {
        font-size: 1.3rem;
        color: #f7f5eb;
        margin-top: 1rem;
        font-family: 'Monaco';
    }

    mark{
        background-color: #5EABE8;
    }



    .img{
        width: 50%;
    }
    
    .title-card {
        background-color: #FFD95C;
        height: 100vh; 
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
        padding: 2rem;
        box-sizing: border-box;
        font-family: "Inter", sans-serif;
    }

    .content {
        max-width: 700px;
        background-color: #E6A84E;
        padding: 2rem;
        border: 6px solid #5EABE8;
        border-radius: 2rem;
        box-shadow: 16px 16px #F0F1F3;
    }



    @media (max-width: 600px) {
        h1 {
            font-size: 2.2rem;
        }

        p {
            font-size: 1.1rem;
        }
    }
</style>
