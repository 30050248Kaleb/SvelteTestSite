<div class="row row-cols-1 row-cols-md-4 g-4">
    {#each superheroes as hero}
    {#if hero.publisher === publisher}
    <div class="col">
    <HeroCard 
    cardColour={publisherColour}
    name={hero.superhero}
    alterEgo={hero.alter_ego}
    firstAppearance={hero.first_appearance}
    characters={hero.characters}
    />
    </div>
    {/if}
{/each}
</div>

<script>
    // Json from https://gist.github.com/mariodev12/a923f2b651a005ca3ca7f851141efcbc
    import superheroes from '../../assets/data/superheroes.json';
    import HeroCard from './HeroCard.svelte';

    export let publisher = 'DC Comics';
    export let publisherColour = 'primary';
</script>

