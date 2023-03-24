<section>
  <div class="about-container">
    <div class="img-placeholder" />
    <div class="about-text-content">
      <p>ABOUT</p>
      <p>
        My name is Gustaf and I am a passionate Front End Developer with a
        strong focus on creating beautiful and user-friendly applications for
        both web and mobile platforms. I love to design prototypes and bring
        them to life with clean and elegant code.
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
    </div>
  </div>
</section>

<style>
  section {
    height: 100vh;
    width: 100%;
    display: grid;
    place-content: center;
  }

  .about-container {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .img-placeholder {
    height: 20rem;
    width: 20rem;
    background: lightskyblue;
    border-radius: 1rem;
  }

  .about-text-content {
    width: 20%;
    padding-left: 10rem;
    margin-bottom: auto;
    cursor: default;
  }

  .text-span {
    font-weight: bold;
    cursor: pointer;
  }

  .text-span a {
    text-decoration: none;
  }
</style>
