<script>
    export let name;
    export let icon;

    import Fa from 'svelte-fa'
    import Term from '../Term.svelte'
</script>

<div class='box content p-0 mx-1 my-2'>
    <div class='columns is-mobile p-0 m-0'>
        <div class='column is-2 p-2 m-0'>
            <Fa class='p-0 m-0' icon={icon} />
        </div>
        <div class='column p-1 m-0 has-text-centered'>
            <h3 class='p-0 m-0'><Term>{name}</Term></h3>
        </div>
    </div>
    <p class='has-text-centered'><slot></slot></p>
</div>

<style lang='scss'>
    p {
        font-size: 75%;
        padding: 0.5rem;
        padding-top: 0;
    }
</style>