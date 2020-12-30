<script>
    import Page from "../Page.svelte"
    export let page;

    import IconBox from 'widgets/IconBox.svelte';
    import {faTruck, faCity, faHandHoldingUsd, faPlane, faShoppingCart, faSkull, faTools, faShieldAlt} from 'icons'
</script>

<Page page={page}>
    <div class='columns is-mobile p-0 m-0'>
        <div class='column m-0 p-0'>
            <IconBox icon={faTruck} name='Hauler'>
                Quick reflexes under pressure.
            </IconBox>
            <IconBox icon={faCity} name='Urchin'>
                Adept at staying out of trouble.
            </IconBox>
            <IconBox icon={faHandHoldingUsd} name='Scab'>
                Betrayer. Safe, secure, surveilled.
            </IconBox>
            <IconBox icon={faPlane} name='Pilot'>
                Fastest thing in the Belt.
            </IconBox>
        </div>
        <div class='column m-0 p-0'>
            <IconBox icon={faShoppingCart} name='Merchant'>
                Always ready to make a deal.
            </IconBox>
            <IconBox icon={faSkull} name='Revenaut'>
                They thought you were dead. Now you're back.
            </IconBox>
            <IconBox icon={faTools} name='Technician'>
                Something's always broken.
            </IconBox>
            <IconBox icon={faShieldAlt} name="Mercenary">
                Loyalty & service. For a price.
            </IconBox>
        </div>
    </div>			
</Page>