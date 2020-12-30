<script>
    import Page from '../Page.svelte';
    export let page;

    import BkgndBox from 'widgets/BkgndBox.svelte'
    import Term from 'widgets/Term.svelte'
    import {faShieldAlt} from 'icons'
</script>

<Page page={page}>
    <BkgndBox name='Mercenary' icon={faShieldAlt}>
        <span slot='bonuses'>
            <p class='is-small'>+3 <Term>Vitality</Term></p>
            <p>+1 <Term>Endure</Term></p>
            <p>+1 <Term>Resist (Phys)</Term></p>
        </span>
        <span slot='incentives'>
            <label>
                <input type='radio'><p>Did I strike first?</p>
            </label>
            <label>
                <input type='radio'><p>Did I earn money?</p>
            </label>
            <label>
                <input type='radio'><p>Did I uphold a code of honor?</p>
            </label>
        </span>
    </BkgndBox>
    <p>You or your folks used to work for Valent keeping the "peace", but now you follow the money. Sometimes you work for Valent, sometimes not. In every case, you find that nothing is more persuasive than the barrel of a gun or an overheating core about to blow. Mercenaries are often covered in scars and tattoos, and can live and work anywhere on Ceres.</p>
</Page>