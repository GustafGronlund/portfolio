<script>
  let toggleWave = false;

  const logoWave = (isWaving) => {
    toggleWave = isWaving;
  };
</script>

<header>
  <div class="spacing" />
  <span class:active={toggleWave}>👋</span>
  <a
    href="/app"
    on:mouseenter={() => logoWave(true)}
    on:mouseleave={() => logoWave(false)}
  >
    Gronlund.dev</a
  >
  <nav>
    <ul>
      <li>About</li>
      <li>Projects</li>
      <li>Skills</li>
      <li>Contact</li>
    </ul>
  </nav>
</header>

<style>
  header {
    position: fixed;
    top: 0;
    display: flex;
    flex-direction: row;
    align-items: center;
    width: 100%;
  }

  .spacing {
    width: 2rem;
  }

  a {
    text-decoration: none;
    color: #282828;
    cursor: pointer;
    font-size: 1em;
    height: fit-content;
    padding: 2rem 0 2rem 0;
    margin-left: 0.5rem;
    font-weight: bold;
  }

  nav {
    padding: 2rem;
    margin-left: auto;
  }

  ul {
    display: flex;
    justify-content: space-between;
    width: 20rem;
    padding: 0;
    margin: 0;
  }

  li {
    list-style: none;
    font-size: 1rem;
    cursor: pointer;
  }

  @keyframes waving {
    0% {
      transform: rotate(0deg);
    }
    25% {
      transform: rotate(-35deg);
    }
    50% {
      transform: rotate(35deg);
    }
    100% {
      transform: rotate(0deg);
    }
  }

  span.active {
    animation-name: waving !important;
    animation-iteration-count: infinite;
    animation-duration: 3s;
  }
</style>
