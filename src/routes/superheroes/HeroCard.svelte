<script>
    export let cardColour = "dark";
    export let name = "";
    export let alterEgo = "";
    export let firstAppearance = "";
    export let characters = "";
</script>

<div class="card h-100 text-white bg-{cardColour}" style="width: 18rem;">
    <div class="card-body">
      <h5 class="card-title">{name}</h5>
      <h6 class="card-subtitle mb-2 text-light">A.K.A. {alterEgo}</h6>
      <p class="card-text"><b>First Appearance:</b> {firstAppearance}.</p>
      <p class="card-text"><b>Characters:</b> {characters}
      </p>
    </div>
  </div>