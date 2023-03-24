<script>
  import ProjectCard from "../shared/ProjectCard.svelte";
</script>

<section>
  <ProjectCard />
  <ProjectCard />
  <ProjectCard />
  <ProjectCard />
</section>

<style>
  section {
    height: 100vh;
    width: 100%;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
  }
</style>
