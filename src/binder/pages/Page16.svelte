<script>
    import Page from '../Page.svelte';
    export let page;

    import Term from '../../Term.svelte'
</script>

<Page page={page}>
    <div id='ad' class='columns is-mobile m-0 p-0' style='position: relative'>
        <div class='column is-2 m-0 p-0'>
            <h2 id='more'><i><strong>more from ceres...</strong></i></h2>
        </div>
        <div class='column m-0 p-0'>
            <div class='box m-2 p-2'>
                <h3 class='p-0 m-0 mb-1'><Term>Places</Term></h3>
                <p>Visit the neighborhoods, streets, and bullet-ridden homes of Ceres station.</p>
            </div>
            <div class='box m-2 p-2'>
                <h3 class='p-0 m-0 mb-1'><Term>People</Term></h3>
                <p>Factions battle for resources while Ceres collapses under their feet. <Term>Valent</Term> oversees all. Meet the people who called Ceres home.</p>
            </div>
            <div class='box m-2 p-2'>
                <h3 class='p-0 m-0 mb-1'><Term>Wield Trees</Term></h3>
                <p>Six <Term>wield trees</Term> for the Ceres setting: the <Term>Hacker</Term>, the <Term>Empath</Term>, the <Term>Engineer</Term>, the <Term>Oracle</Term>, and the <Term>Biotic</Term></p>
            </div>
            <div class='box m-2 p-2'>
                <h3 class='p-0 m-0 mb-1'><Term>Artifacts & Arms</Term></h3>
                <p>Items for heroes and villians, crafted or encountered by the people of Ceres.</p>
            </div>
        </div>
    </div>
</Page>

<style>
    #ad p {
		font-size: 75%;
	}

	#more {
		position: absolute;
		transform-origin: top left;
		transform: rotate(270deg);
		top: 12rem;
	}
</style>