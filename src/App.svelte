<script>
  import "@fontsource/open-sans";
  import Navigation from "./components/Navigation.svelte";
  import AboutSection from "./components/AboutSection.svelte";
  import ProjectsSection from "./components/ProjectsSection.svelte";
  import TechStackSection from "./components/TechStackSection.svelte";
  import ContactSection from "./components/ContactSection.svelte";
  import ScrollingIndicator from "./shared/ScrollingIndicator.svelte";
  import SocialMediaIcon from "./shared/SocialMediaIcon.svelte";
</script>

<Navigation />
<main>
  <section class="hero">
    <div class="hero-content">
      <article class="text-content">
        <h1>Gustaf Grönlund</h1>
        <p>
          Front End Developer <br />based in Malmö, Sweden.
        </p>
        <section class="social-media-icons">
          <SocialMediaIcon />
          <SocialMediaIcon />
        </section>
      </article>
      <img
        src="../public/img/profile_picture.jpg"
        alt="A profile picture of me."
      />
    </div>
  </section>
  <AboutSection />
  <ProjectsSection />
  <TechStackSection />
  <ContactSection />
</main>
<ScrollingIndicator />

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
    padding-right: 4rem;
  }

  .text-content h1 {
    font-size: 4rem;
    background-image: linear-gradient(90deg, #ea99da 0%, #5d6cf9 100%);
    background-clip: text;
    -webkit-background-clip: text;
    color: transparent;
    margin: 0;
  }

  .text-content p {
    font-size: 2rem;
    margin-top: 0.5rem;
  }

  .social-media-icons {
    display: flex;
    flex-direction: row;
    width: 100%;
  }

  .social-media-icons .icon-container:nth-child(1) {
    margin-right: 2rem;
  }

  img {
    width: 20%;
    border-radius: 50%;
  }

  @media (max-width: 650px) {
    .hero-content {
      flex-direction: column-reverse;
      gap: 2rem;
    }

    img {
      width: 60%;
    }

    .text-content {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      padding-right: 0rem;
    }

    .text-content h1 {
      font-size: 2rem;
    }

    .text-content p {
      font-size: 1rem;
      text-align: center;
    }
  }
</style>
