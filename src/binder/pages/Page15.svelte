<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from 'widgets/BkgndBox.svelte'
    import Term from 'widgets/Term.svelte'
    import {faPlane} from 'icons'
</script>

<Page page={page}>
    <BkgndBox name='Pilot' icon={faPlane}>
        <span slot='bonuses'>
            <p class='is-small'>+3 <Term>Vitality</Term></p>
            <p>+1 <Term>Endure</Term></p>
            <p>+1 <Term>Resist (Phys)</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I perform under pressure?</p>
            </label>
            <label>
                <input type='radio'><p>Did I make a harrowing escape?</p>
            </label>
            <label>
                <input type='radio'><p>Did I tell a story about my exploits?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You can fly anything. You have an intuitive understanding of machines, but specialize in the "duct tape and prayers" school of repair. Pilots can be cocky and self-assured, but their confidence is often earned through harrowing brushes with death. </p>
</Page>