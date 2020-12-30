<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from 'widgets/BkgndBox.svelte'
    import Term from 'widgets/Term.svelte';
    import {faShoppingCart} from 'icons'
</script>

<Page page={page}>
    <BkgndBox name='Merchant' icon={faShoppingCart}>
        <span slot='bonuses'>
            <p class='is-small'>+2 <Term>Tenacity</Term></p>
            <p>+1 <Term>Notice</Term></p>
            <p>+3 in <Term>2 lang</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I make a deal?</p>
            </label>
            <label>
                <input type='radio'><p>Did I charm someone out of treasure?</p>
            </label>
            <label>
                <input type='radio'><p>Did I avoid arousing suspicion?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You are most at home on the Ceres docks, where you trade with Haulers and Voidwalkers who bring tales and goods from all around the system. People who have been out in space can be... strange, but you're more than capable of charming anything with a pulse and a paycheck.</p>
</Page>