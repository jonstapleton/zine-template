<script>
    import Page from '../Page.svelte';
    import BkgndBox from '../../widgets/BkgndBox.svelte';
    import Term from '../../Term.svelte'
    export let page;

    import {faHandHoldingUsd} from '@fortawesome/free-solid-svg-icons';
</script>

<Page page={page}>
    <BkgndBox name='Scab' icon={faHandHoldingUsd}>
        <span slot='bonuses'>
            <p class='is-small'>+2 <Term>Vigilance</Term></p>
            <p>+2 <Term>Vitality</Term></p>
            <p>+1 <Term>Recall (Hist)</Term> or <Term>(Pol)</Term></p>
            <p>+1 <Term>Resist (Mental)</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I take a risk to satisfy my curiosity?</p>
            </label>
            <label>
                <input type='radio'><p>Did I learn a secret about someone?</p>
            </label>
            <label>
                <input type='radio'><p>Did I stand up to someone in authority?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You live in Elysium, the beautiful ring of homes, parks, and gardens on the outer edge of Ceres along the equator. You've lived your life in relative comfort, but under the heavy thumb and all-seeing eye of Valent and its police.</p>
</Page>