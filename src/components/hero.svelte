
<script>
    import 'animate.css';
</script>


<div class="image_hero">
    <div id="triangle_container">
        <div id="triangle"></div>
    </div>
    <div id="square_container">
        <div id="square"></div>
    </div>
    <div id="circle_container">
        <div id="circle"></div>
    </div>
</div>
<div id="text_container">
    <h1 style="color: #74a466" class="large_text animate__animated animate__fadeInLeft">Ludwig Lechtreck</h1>
</div> 


<style>
 @keyframes fadeIn {
        0% { opacity: 0; }
        100% { opacity: 1; }
    }
.image_hero {
        display: flex;
        justify-content: center;
        flex-direction: row;
    }
    #triangle {
        width: 0;
        height: 0;
        border-left: 100px solid transparent;
        border-right: 100px solid transparent;
        border-bottom: 200px solid #444795;
        animation: fadeIn 3s;
    }
    #square {
        width: 200px;
        height: 200px;
        background: #E74536;
        animation: fadeIn 4s;
    }
    #circle {
        width: 200px;
        height: 200px;
        background: #FFC915;
        border-radius: 50%;
        animation: fadeIn 5s;
    }
    #triangle_container{
        padding-right: 100px;
    }
    #square_container {
        padding-right: 100px;
        padding-left: 100px;
    }
    #circle_container {
        padding-left: 100px;
    }

    #text_container {
        padding-top: 100px;
        display: flex;
        align-items: left;
        justify-content: space-between;
        flex-direction: column;
        padding-left: 15em;
    }
    .large_text {
       font-size: 5em;
    }
    .small_text {
        font-size: 2em;
    }
    
</style>