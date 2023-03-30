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
    grid-column-gap: 3rem;
    grid-row-gap: 3rem;
  }

  @media (max-width: 650px) {
    section {
      display: flex;
      flex-direction: column;
      padding: 0 1rem 0 1rem;
      min-width: 100vh;
    }
  }
</style>
