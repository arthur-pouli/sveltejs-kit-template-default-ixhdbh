<script>
  import { page } from '$app/stores';
  import bornes from '$lib/listing.js'

  let borne = bornes.find(borne => borne.id === parseInt($page.params.id))
   
</script>

{#if borne}
  <div>{borne.name}</div>
{/if}
