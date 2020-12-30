<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from '../../widgets/BkgndBox.svelte';
    import Term from '../../Term.svelte';

    import {faTruck} from '@fortawesome/free-solid-svg-icons';
</script>

<Page page={page}>
    <BkgndBox name='Hauler' icon={faTruck}>
        <span slot='bonuses'>
            <p class='is-small'>+2 <Term>Tenacity</Term></p>
            <p>+2 <Term>Vitality</Term></p>
            <p>+1 <Term>Stabilize</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I take a risk?</p>
            </label>
            <label>
                <input type='radio'><p>Did I break something?</p>
            </label>
            <label>
                <input type='radio'><p>Did I perform under pressure?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You work on a long-haul freighter, breaking chunks of ice and other valuable materials off of asteroids in the Belt. You have quick reflexes and steady nerves under pressure. You are used to backbreaking, nerve-shredding work where one unsure movement means the difference between returning in one piece ending up as a ball of frozen gore.</p>
</Page>
