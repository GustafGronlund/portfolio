<script>
  import { Lottie } from "lottie-svelte";
</script>

<section class="about-container">
  <figure class="svg-container">
    <Lottie path="../public/json/programming.json" speed={1} />
  </figure>
  <article class="about-text-content">
    <p>
      My name is Gustaf and I am a passionate Front End Developer with a strong
      focus on creating beautiful and user-friendly applications for both web
      and mobile platforms. I love to design prototypes and bring them to life
      with clean and elegant code.
    </p>

    <p>
      Aside from my love for programming, I am also an avid coffee drinker and
      enjoy cooking and trying out new recipes. In my spare time, I am a
      musician and music producer. I play in a <span class="text-span"
        ><a
          href="https://open.spotify.com/artist/4SHgev36xbbgjVsLRXVMsm?si=hiR-TLLwRd6uiGfbpEKVNw"
          target="_blank">post-punk</a
        ></span
      >
      band as well as an
      <span class="text-span"
        ><a
          href="https://open.spotify.com/artist/2SEHhzHhXEADDOfiajcQDa?si=OAiIFwppRpKiaL8v6cQXoA"
          target="_blank">indie-pop</a
        ></span
      >
      band, and you can check out some of my production work
      <span class="text-span"
        ><a
          href="https://open.spotify.com/artist/5Ppg5BLRRTBZ7mDkVaaAVz?si=hPSyf08BSymLXJpV1hLZLA"
          target="_blank">here</a
        ></span
      >.
    </p>
  </article>
</section>

<style>
  .about-container {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .svg-container {
    height: 20rem;
    width: 20rem;
  }

  .about-text-content {
    width: 30%;
    padding-left: 10rem;
    cursor: default;
  }

  .text-span {
    font-weight: bold;
    cursor: pointer;
  }

  .text-span a {
    text-decoration: none;
  }

  @media (max-width: 650px) {
    .svg-container {
      height: 15rem;
      width: 15rem;
    }

    .about-container {
      flex-direction: column;
    }

    .about-text-content {
      width: 100%;
      padding-left: 0rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .about-text-content p {
      margin: 0 1rem 0 1rem;
    }
  }
</style>
