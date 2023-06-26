<script lang="ts">
	export let bullets: string[];
</script>

<ul>
	{#each bullets as bullet}
		<li class="bullet_item">{bullet}</li>
	{/each}
</ul>

<style>
    .bullet_item {
        font-size: 24pt;
        padding-bottom: 3em;
    }

</style>