<script lang="ts">
    import Unorderedlist from "./unorderedlist.svelte";
    export let image: string;
    export let company: string;
    export let title_date: string;
    export let desc: string[];

</script>

<div class="exp_container">
    <div class="facts_container">
        <img class="company_logo" alt="company_logo" src={image} />
        <h1  style="font-size: 26pt" class="company_name">{company}</h1>
        <h3 class="company_title">{title_date}</h3>
    </div>
    <div class="bullet_container">
        <Unorderedlist bullets={desc} />
    </div>
</div>


<style>
      .facts_container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        padding-right: 3em;
    }
    .exp_container {
        display: flex;
        flex-direction: row;
        padding-left: 2em;
        align-items: center;
    } 
     .company_logo {
        width: var(--img_width);
        height: var(--img_height)
    }
    .bullet_container {
        padding-top: 6em;
    }
  
</style>