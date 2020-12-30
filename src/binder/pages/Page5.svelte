<script>
    import Page from '../Page.svelte';
    export let page;

    import Term from 'widgets/Term.svelte';
    import BkgndBox from "widgets/BkgndBox.svelte";
    import {faCity} from 'icons';
</script>

<Page page={page}>
    <BkgndBox name='Urchin' icon={faCity}>
        <span slot='bonuses'>
            <p class='is-small'>+4 <Term>Vigilance</Term></p>
            <p>+1 <Term>Notice</Term></p>
            <p>+1 <Term>Navigate</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I get in and out without being seen?</p>
            </label>
            <label>
                <input type='radio'><p>Did I gather info without revealing myself?</p>
            </label>
            <label>
                <input type='radio'><p>Did I manipulate my enemy for an advantage?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You're most at home in the cramped, greasy tunnels at the center of your station. Everyone you know grew up in low gravity, and your body is adapted to these conditions. Your home is dangerous and unpredictable, but you're adept at keeping yourself out of trouble (or at least making trouble for others). </p>
</Page>