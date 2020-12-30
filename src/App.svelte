<script>
	import Term from './Term.svelte';
	import BkgndBox from './widgets/BkgndBox.svelte'
	import IconBox from './widgets/IconBox.svelte';
	import {faTruck, faCity, faHandHoldingUsd, faPlane, faShoppingCart, faSkull, faTools, faShieldAlt} from '@fortawesome/free-solid-svg-icons'
</script>

<main class="zine">
	<section class="zine-page page-1">
		<h1>Cover Page</h1>
	</section>
	<section class="zine-page page-1b content is-small">
		<h1 class='title'><Term>Backgrounds</Term></h1>
		<blockquote>A <Term>background</Term> grants a character relatively
			minor adjustments to <Term>attributes</Term>, <Term>skills</Term>, and
			<Term>abilities</Term>, and it determines one of the
			character’s <Term>incentives</Term>.
		</blockquote>
		<p>The <Term>backgrounds</Term> in this package represent characters' connections to different communities on Ceres Station. Your character's background may have an impact on their upbringing, worldview, or social connections. Most <Term>NPCS</Term> also have a <Term>background</Term>.</p>
	</section>
	<section class="zine-page page-2 content is-small">
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
	</section>
	<section id='hauler' class="zine-page page-2b content is-small">
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
	</section>
	<section id='urchin' class="zine-page page-3 content is-small">
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
	</section>
	<section class="zine-page page-3b">
		<h1>Urchin Art</h1>
	</section>
	<section id='scab' class="zine-page page-4 content is-small">
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
	</section>
	<section id='scab' class="zine-page page-4b">
		<h1>Scab Art</h1>
	</section>
	<section class="zine-page page-5 content is-small">
		<BkgndBox name='Merchant' icon={faShoppingCart}>
			<span slot='bonuses'>
				<p class='is-small'>+2 <Term>Tenacity</Term></p>
				<p>+1 <Term>Notice</Term></p>
				<p>+3 in <Term>2 lang</Term></p>
			</span>
			<span slot='incentives'>
				<label>
					<input type='radio'><p>Did I make a deal?</p>
				</label>
				<label>
					<input type='radio'><p>Did I charm someone out of treasure?</p>
				</label>
				<label>
					<input type='radio'><p>Did I avoid arousing suspicion?</p>
				</label>
			</span>
		</BkgndBox>
		<p>You are most at home on the Ceres docks, where you trade with Haulers and Voidwalkers who bring tales and goods from all around the system. People who have been out in space can be... strange, but you're more than capable of charming anything with a pulse and a paycheck.</p>
	</section>
	<section class="zine-page page-5b">
		<h1>Merchant Art</h1>
	</section>
	<section id='revenaut' class="zine-page page-6 content is-small">
		<BkgndBox name='Revenaut' icon={faSkull}>
			<span slot='bonuses'>
				<p class='is-small'>+3 <Term>Vig</Term> or <Term>Ten</Term> or <Term>Vit</Term></p>
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
		<p>You've seen between the folds of the inky abyss, and have wrapped yourself in its icy embrace. Revenauts are those who were lost, abandoned, or trapped out in space. They left part of themselves out there, and brought back a piece of the void in its place. Some are just odd, but others wield mysterious powers, unexplainable insights, or artifacts of unknown origin.</p>
	</section>
	<section class="zine-page page-6b">
		<h1>Page 6</h1>
	</section>
	<section id='technician' class="zine-page page-7 content is-small">
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
	</section>
	
	<section id='mercenary' class="zine-page page-7b content is-small">
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
	</section>
	<section class="zine-page page-8 content is-small">
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
	</section>

	<section  id='ad' class="zine-page page-8b content is-small">
		<div class='columns is-mobile m-0 p-0' style='position: relative'>
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
	</section>
</main>

<style lang="scss">
	@import 'bulma/bulma.sass';

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
