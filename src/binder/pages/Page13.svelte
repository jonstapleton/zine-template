<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from '../../widgets/BkgndBox.svelte'
    import Term from '../../Term.svelte'
    import {faTools} from '@fortawesome/free-solid-svg-icons'
</script>

<Page page={page}>
    <BkgndBox name='Technician' icon={faTools}>
        <span slot='bonuses'>
            <p class='is-small'>+4 <Term>Tenacity</Term></p>
            <p>+2 <Term>Fabricate</Term></p>
            <p>+1 <Term>Hack</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I misuse technology to achieve my goals?</p>
            </label>
            <label>
                <input type='radio'><p>Did I take or complete a contract?</p>
            </label>
            <label>
                <input type='radio'><p>Did I make something new?</p>
            </label>
        </span>
    </BkgndBox>
    <p>Technicians find themselves in every part of Ceres, repairing, replacing, and occasionally sabotaging the systems that make Ceres run. You can always find someone willing to throw you some cash for an odd job, and you have contacts from all over. </p>
</Page>