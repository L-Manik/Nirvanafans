<script lang="ts">
    import Icon from "svelte-awesome";
    import type {IconType} from "svelte-awesome/components/Icon-svelte"

    export let iconData: IconType;
    export let title: string
</script>

<div class="container">
    <div class="section-title">
        <Icon data={iconData} />
        {title}
    </div>
    <slot/>
</div>

<style>
    .container { 
        display: flex;
        flex-direction: column;
        gap: 16px;
    }
    .section-title {
		background-color: #ffeb3b;
		border-left: solid 4px #fbc02d;
		padding: 8px 16px;
		text-transform: UPPERCASE;
		font-weight: 500;
		margin: 16px 0px;
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 1rem;
	}
</style>