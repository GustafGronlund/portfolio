<script>
  import "@fontsource/open-sans";
  import Navigation from "./components/Navigation.svelte";
  import AboutSection from "./components/AboutSection.svelte";
  import ProjectsSection from "./components/ProjectsSection.svelte";
  import TechStackSection from "./components/TechStackSection.svelte";
  import ContactSection from "./components/ContactSection.svelte";
</script>

<Navigation />
<main>
  <section class="hero">
    <div class="hero-content">
      <div class="text-content">
        <h1>Gustaf Grönlund</h1>
        <p>
          Front End Developer <br />based in Malmö,
          <span class="country-span">Sweden</span>.
        </p>
        <div class="social-media-icons">
          <div class="icon-container">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="32"
              height="32"
              viewBox="0 0 256 256"
              ><path
                fill="#0A66C2"
                d="M218.123 218.127h-37.931v-59.403c0-14.165-.253-32.4-19.728-32.4c-19.756 0-22.779 15.434-22.779 31.369v60.43h-37.93V95.967h36.413v16.694h.51a39.907 39.907 0 0 1 35.928-19.733c38.445 0 45.533 25.288 45.533 58.186l-.016 67.013ZM56.955 79.27c-12.157.002-22.014-9.852-22.016-22.009c-.002-12.157 9.851-22.014 22.008-22.016c12.157-.003 22.014 9.851 22.016 22.008A22.013 22.013 0 0 1 56.955 79.27m18.966 138.858H37.95V95.967h37.97v122.16ZM237.033.018H18.89C8.58-.098.125 8.161-.001 18.471v219.053c.122 10.315 8.576 18.582 18.89 18.474h218.144c10.336.128 18.823-8.139 18.966-18.474V18.454c-.147-10.33-8.635-18.588-18.966-18.453"
              /></svg
            >
          </div>
          <div class="icon-container">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="32"
              height="32"
              viewBox="0 0 256 256"
              ><g fill="none"
                ><rect width="256" height="256" fill="#242938" rx="60" /><path
                  fill="#fff"
                  d="M128.001 30C72.779 30 28 74.77 28 130.001c0 44.183 28.653 81.667 68.387 94.89c4.997.926 6.832-2.169 6.832-4.81c0-2.385-.093-10.262-.136-18.618c-27.82 6.049-33.69-11.799-33.69-11.799c-4.55-11.559-11.104-14.632-11.104-14.632c-9.073-6.207.684-6.079.684-6.079c10.042.705 15.33 10.305 15.33 10.305c8.919 15.288 23.394 10.868 29.1 8.313c.898-6.464 3.489-10.875 6.349-13.372c-22.212-2.529-45.56-11.104-45.56-49.421c0-10.918 3.906-19.839 10.303-26.842c-1.039-2.519-4.462-12.69.968-26.464c0 0 8.398-2.688 27.508 10.25c7.977-2.215 16.531-3.326 25.03-3.364c8.498.038 17.06 1.149 25.051 3.365c19.087-12.939 27.473-10.25 27.473-10.25c5.443 13.773 2.019 23.945.98 26.463c6.412 7.003 10.292 15.924 10.292 26.842c0 38.409-23.394 46.866-45.662 49.341c3.587 3.104 6.783 9.189 6.783 18.519c0 13.38-.116 24.149-.116 27.443c0 2.661 1.8 5.779 6.869 4.797C199.383 211.64 228 174.169 228 130.001C228 74.771 183.227 30 128.001 30ZM65.454 172.453c-.22.497-1.002.646-1.714.305c-.726-.326-1.133-1.004-.898-1.502c.215-.512.999-.654 1.722-.311c.727.326 1.141 1.01.89 1.508Zm4.919 4.389c-.477.443-1.41.237-2.042-.462c-.654-.697-.777-1.629-.293-2.078c.491-.442 1.396-.235 2.051.462c.654.706.782 1.631.284 2.078Zm3.374 5.616c-.613.426-1.615.027-2.234-.863c-.613-.889-.613-1.955.013-2.383c.621-.427 1.608-.043 2.236.84c.611.904.611 1.971-.015 2.406Zm5.707 6.504c-.548.604-1.715.442-2.57-.383c-.874-.806-1.118-1.95-.568-2.555c.555-.606 1.729-.435 2.59.383c.868.804 1.133 1.957.548 2.555Zm7.376 2.195c-.242.784-1.366 1.14-2.499.807c-1.13-.343-1.871-1.26-1.642-2.052c.235-.788 1.364-1.159 2.505-.803c1.13.341 1.871 1.252 1.636 2.048Zm8.394.932c.028.824-.932 1.508-2.121 1.523c-1.196.027-2.163-.641-2.176-1.452c0-.833.939-1.51 2.134-1.53c1.19-.023 2.163.639 2.163 1.459Zm8.246-.316c.143.804-.683 1.631-1.864 1.851c-1.161.212-2.236-.285-2.383-1.083c-.144-.825.697-1.651 1.856-1.865c1.183-.205 2.241.279 2.391 1.097Z"
                /></g
              ></svg
            >
          </div>
        </div>
      </div>
      <img src="../public/img/profile_picture.jpg" alt="profile_picture" />
    </div>
  </section>
  <AboutSection />
  <ProjectsSection />
  <TechStackSection />
  <ContactSection />
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

  .country-span {
    background-image: linear-gradient(90deg, #006aa8 0%, #fecd00 100%);
    background-clip: text;
    -webkit-background-clip: text;
    color: transparent;
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

  .icon-container {
    height: 4rem;
    width: 4rem;
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    box-shadow: 0 0 15px 1px rgba(0, 0, 0, 0.05);
    cursor: pointer;
    transition: all 0.3s ease-in-out;
  }

  .icon-container:hover {
    transform: scale(1.1);
  }

  img {
    width: 20%;
    border-radius: 50%;
  }
</style>
