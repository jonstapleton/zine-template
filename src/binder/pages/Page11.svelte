<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from 'widgets/BkgndBox.svelte';
    import Term from 'widgets/Term.svelte';
    import {faSkull} from 'icons'
</script>

<Page page={page}>
    <BkgndBox name='Revenaut' icon={faSkull}>
        <span slot='bonuses'>
            <p class='is-small m-0 p-0'>+3 <Term>Vig</Term> or <Term>Ten</Term> or <Term>Vit</Term></p>
            <p>+1 <Term>Resist (Mental)</Term></p>
            <p>+1 <Term>Endure</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I overcome the odds?</p>
            </label>
            <label>
                <input type='radio'><p>Did I draw on my experience being stranded?</p>
            </label>
            <label>
                <input type='radio'><p>Did I express my resilience?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You've seen between the folds of the inky abyss, and have wrapped yourself in its icy embrace. Revenauts were once lost, abandoned, or trapped alone out in space. They left part of themselves out there, and brought back a piece of the void in its place. Some are just odd; others wield strange powers, uncanny foresight, or artifacts of unknown origin.</p>
</Page>