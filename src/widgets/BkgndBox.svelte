<script>
    import Fa from 'svelte-fa';
    import Term from '../Term.svelte';
    export let icon;
    export let name;
</script>

<div class='box content'>
    <div class='level mb-2 is-mobile'>
        <div class='level-item'>
            <Fa size='1.5x' icon={icon} />
        </div>
        <div class='level-item has-text-centered'>
            <h3 class='pt-1'><Term>{name}</Term></h3>
        </div>
        <div class='level-item'>
            <slot name='bonuses'></slot>
        </div>
    </div>
    <div id='incentives'>
        <p id='label'><i><strong>incentives</strong></i></p>
        <div class='field'>
            <slot name='incentives'></slot>
        </div>
    </div>
</div>

<style lang='scss'>
    @import 'bulma/bulma.sass';

    div :global(p){
        font-size: 75%;
        @extend .p-0, .m-0;
    }

    #incentives {
        position: relative;
        top: -0.2rem;
    }

    #label {
        position: absolute;
        transform: rotate(270deg) translateX(-2.85rem);
        transform-origin: top left;
    }

    .field {
        margin-left: 10px;
    }

    .field :global(input) {
        width: 2em;
        height: 1em;
        display: inline-block;
        position: relative;
        top: 2px;
    }

    .field :global(p) {
        display: inline-block;
        position: static;
        left: 2rem;
        font-size: 60%;
    }
</style>