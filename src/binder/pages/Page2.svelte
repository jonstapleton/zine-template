<script>
    import Term from '../../Term.svelte';
    import Page from '../Page.svelte';
    export let page;
</script>

<Page page={page}>
    <h1 class='title'><Term>Backgrounds</Term></h1>
    <blockquote>A <Term>background</Term> grants a character relatively
        minor adjustments to <Term>attributes</Term>, <Term>skills</Term>, and
        <Term>abilities</Term>, and it determines one of the
        character’s <Term>incentives</Term>.
    </blockquote>
    <p>The <Term>backgrounds</Term> in this package represent characters' connections to different communities on Ceres Station. Your character's background may have an impact on their upbringing, worldview, or social connections. Most <Term>NPCS</Term> also have a <Term>background</Term>.</p>
</Page>