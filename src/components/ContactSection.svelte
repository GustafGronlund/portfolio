<script>
  let buttonHover = false;

  const toggleButton = () => {
    buttonHover = !buttonHover;
  };
</script>

<section>
  <img src="../public/img/cat_typing.gif" alt="cat typing" />
  <footer>
    <div class="footer-text-content">
      <h1>
        Have a passion project or a big idea brewing? Let's spark some
        collaboration and bring your vision to life. 😊
      </h1>
    </div>
    <div class="contact-content">
      <button
        on:mouseenter={() => toggleButton()}
        on:mouseleave={() => toggleButton()}
        ><span class="button-content"
          >Drop me a line<span
            ><div class:active={buttonHover}>
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="0.5rem"
                height="0.5rem"
                viewBox="0 0 24 24"
                class:activeIcon={buttonHover}
                ><path
                  fill="currentColor"
                  d="M12 22q-2.05 0-3.875-.788t-3.188-2.15q-1.362-1.362-2.15-3.187T2 12q0-2.075.788-3.888t2.15-3.174Q6.3 3.575 8.124 2.788T12 2q2.075 0 3.888.788t3.174 2.15q1.363 1.362 2.15 3.175T22 12v1.45q0 1.475-1.012 2.513T18.5 17q-.9 0-1.675-.4t-1.275-1.05q-.675.675-1.588 1.063T12 17q-2.075 0-3.538-1.463T7 12q0-2.075 1.463-3.538T12 7q2.075 0 3.538 1.463T17 12v1.45q0 .725.45 1.137T18.5 15q.6 0 1.05-.413T20 13.45V12q0-3.275-2.363-5.638T12 4Q8.725 4 6.362 6.363T4 12q0 3.275 2.363 5.638T12 20h4q.425 0 .713.288T17 21q0 .425-.288.713T16 22h-4Zm0-7q1.25 0 2.125-.875T15 12q0-1.25-.875-2.125T12 9q-1.25 0-2.125.875T9 12q0 1.25.875 2.125T12 15Z"
                /></svg
              >
            </div></span
          ></span
        ></button
      >
    </div>
  </footer>
</section>

<style>
  section {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }

  section img {
    width: 20%;
    border-radius: 1rem;
    margin-top: auto;
  }

  footer {
    margin-top: auto;
    width: 100vw;
    display: flex;
  }

  .footer-text-content {
    width: 50%;
    padding-left: 2rem;
    padding-bottom: 2rem;
  }

  h1 {
    font-size: 4rem;
    margin: 0;
  }

  .contact-content {
    display: grid;
    place-content: center;
    width: 50%;
  }

  button {
    width: 15rem;
    height: 3rem;
    padding: 0.5rem 2rem 0.5rem 2rem;
    border-radius: 1rem;
    cursor: pointer;
    background: #353535;
    color: #f8f8f8;
    border: none;
  }

  .button-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  button div {
    height: 1rem;
    width: 1rem;
    background: #f8f8f8;
    border-radius: 50%;
    transition: 0.3s all ease-in-out;
  }

  .active {
    transform: scale(2.25);
    display: flex;
    justify-content: center;
    align-items: center;
  }

  svg {
    transition: 0.6s all ease-in-out;
    height: 0.5rem;
    width: 0.5rem;
    opacity: 0;
  }

  .activeIcon {
    opacity: 1;
    color: black;
  }
</style>
