<script>
    import Term from 'widgets/Term.svelte';

    export let name;
    export let level = 0;

    let xp = 0;
    switch(level) {
        case '0':
        case '2':
            xp = 5
            break
        case '1':
            xp = 3
            break
        case '3':
        case '4':
            xp = 8
            break
        default:
            xp = '?'
    }
</script>

<div class='level-{level} box content is-small mx-0 my-3 px-2 pt-0 pb-2'>
    <div class='columns is-mobile m-0 p-0'>
        <div class='column m-0 p-0'>
            <h3 class='m-0 py-2 px-0'><Term>{name}</Term></h3>
        </div>
        <div class='column is-4 m-0 p-1 has-text-right'>
            <p class='info m-0 mt-1 p-0'><i><Term>lvl {level} — {xp} XP</Term></i></p>
        </div>
    </div>
    <p class='description'><slot></slot></p>
</div>

<style>
    .description {
        font-size: 80%;
    }
    .level-0 {
        background-color: white;
    }
    .level-1 {
        background-color: #f3f3f3ff;
    }
    .level-2 {
        background-color: #ccccccff;
    }
    .level-3 {
        background-color: #999999ff;
    }
    .level-3 .description, .level-3 h3 :global(span) {
        color: white;
    }
    .level-4 {
        background-color: #434343ff;
    }
    .level-4 .description, .level-4 h3 :global(span) {
        color: white;
    }
    .info {
        font-size: 100%;
    }
    .level-0 .info {
        color: grey;
    }
    .level-1 .info {
        color: grey;
    }
    .level-2 .info {
        color: #434343ff;
    }
    .level-3 .info {
        color: #f3f3f3ff;
    }
    .level-4 .info {
        color: grey;
    }
</style>