<script context="module">
  export async function preload(page) {
    return { state: page.params["state"] };
  }
</script>

<script>
  import CovidStat from "../components/CovidStat.svelte";
  import CovidChart from "../components/CovidChart.svelte";
  import TableContainer from "../components/TableContainer.svelte";
  export let state;
</script>

<style>

</style>

<svelte:head>
  <title>Covid-19 on {state}</title>
</svelte:head>
<div class="container">
  <div class="row">
    <h1 class="col text-center">Covid-19 on {state}</h1>
  </div>
</div>
