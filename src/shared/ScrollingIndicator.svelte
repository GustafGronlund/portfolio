<script>
  let userIsScrolling = false;

  window.onscroll = (e) => {
    console.log(e);
    scrollRotate();
  };

  const scrollRotate = () => {
    let image = document.querySelector(".scroll-indicator");
    image.style.transform = "rotate(" + window.pageYOffset / 2 + "deg)";
  };
</script>

<div class="scroll-indicator">
  <svg
    xmlns="http://www.w3.org/2000/svg"
    width="32"
    height="32"
    viewBox="0 0 24 24"
    ><path
      fill="currentColor"
      d="m20 12l-1.41-1.41L13 16.17V4h-2v12.17l-5.58-5.59L4 12l8 8l8-8z"
    /></svg
  >
</div>

<style>
  div {
    background: #353535;
    border-radius: 50%;
    height: 4rem;
    width: 4rem;
    position: fixed;
    bottom: 0;
    right: 0;
    margin: 0 2rem 2rem 0;
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0.4;
  }

  svg {
    color: #f8f8f8;
  }

  .scroll-indicator {
    transition: all ease-in-out;
  }
</style>
