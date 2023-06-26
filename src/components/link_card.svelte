<script lang="ts">
    export let image: string;
    export let link_name: string;
    export let link: string;
</script>
<div class="card_container">
    <a class="link_container" href={link}>
        <img class="link_img" alt="link" src={image} />
        <div class="link_text_container">
            <h1>{link_name}</h1>
        </div>
        
    </a>
</div>
<style>
    .link_img {
        width: 15em;
        height: 15em;
    }
    .link_container {
        text-decoration: none;
        color: black;
    }
    .card_container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-left: 5em;
        width: 15em;
        height: 15em;
        padding-top: 5em;
    }
    .link_text_container {
       display: flex;
       flex-direction: row;
       justify-content: center;

    }
</style>