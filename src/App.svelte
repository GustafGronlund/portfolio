<script>
  import "@fontsource/open-sans";
  import Navigation from "./components/Navigation.svelte";
  import TechStackSection from "./components/TechStackSection.svelte";
</script>

<Navigation />
<main>
  <section class="hero">
    <div class="hero-content">
      <div class="text-content">
        <h1>Gustaf Grönlund -</h1>
        <p>Front End Developer based in Malmö</p>
      </div>
      <img src="../public/img/profile_picture.jpg" alt="profile_picture" />
    </div>
  </section>
  <section class="about" />
  <section class="projects" />
  <TechStackSection />
  <section class="contact" />
</main>

<style>
  .hero {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .hero-content {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .text-content {
    display: flex;
    flex-direction: column;
    padding-right: 4rem;
  }

  .text-content h1 {
    font-size: 4rem;
  }

  .text-content p {
    font-size: 1.5rem;
  }

  img {
    width: 20%;
    border-radius: 50%;
    box-shadow: 0 0 10px 3px rgba(0, 0, 0, 0.2);
  }

  .about {
    height: 100vh;
    width: 100%;
    background: beige;
  }

  .projects {
    height: 100vh;
    width: 100%;
    background: lightblue;
  }

  .tech-stack {
    height: 100vh;
    width: 100%;
    background: lightcoral;
  }

  .contact {
    height: 100vh;
    width: 100%;
    background: lightsalmon;
  }
</style>
