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
    class="logo"
  >
    Gronlund.dev</a
  >
  <nav>
    <ul>
      <li><a href="" on:click|preventDefault={() => {}}>About</a></li>
      <li><a href="" on:click|preventDefault={() => {}}>Projects</a></li>
      <li><a href="" on:click|preventDefault={() => {}}>Skills</a></li>
      <li><a href="" on:click|preventDefault={() => {}}>Contact</a></li>
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

  .logo {
    font-weight: bold;
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
    display: inline-block;
  }

  a {
    position: relative;
    display: block;
    cursor: pointer;
    padding: 8px 0;
    color: #353535;
    text-decoration: none;
  }

  a:hover {
    color: #353535;
    text-decoration: none;
  }

  a:before,
  a:after {
    content: "";
    position: absolute;
    width: 0%;
    height: 2px;
    bottom: -2px;
    background: #353535;
  }

  a:before {
    left: 0;
  }
  a:after {
    right: 0;
    background: #353535;
    transition: width 0.8s cubic-bezier(0.22, 0.61, 0.36, 1);
  }

  a:hover:before {
    background: #353535;
    width: 100%;
    transition: width 0.5s cubic-bezier(0.22, 0.61, 0.36, 1);
  }

  a:hover:after {
    background: transparent;
    width: 100%;
    transition: 0s;
  }

  @keyframes waving {
    0% {
      transform: rotate(0deg);
    }
    25% {
      transform: rotate(-20deg);
    }
    75% {
      transform: rotate(20deg);
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
