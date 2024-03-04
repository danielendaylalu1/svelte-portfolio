<script lang="ts">
  import Logo from "../asset/profile.png";
  const navLinks: string[] = ["Home", "Aboutme", "Showcase"];
</script>

<main class="main">
  <section class="navbar">
    <a class="logo" href={``}>D.E</a>
    <ul class="nav">
      {#each navLinks as link (link)}
        <li class="nav-item">
          <a href={`#${link}`} class="nav-link">{link}</a>
        </li>
      {/each}
    </ul>
    <ul class="nav navbar-social-links">
      <li class="nav-item">
        <a href={`#`} class="nav-link"
          ><i class="fa-brands fa-linkedin-in"></i></a
        >
      </li>
      <li class="nav-item">
        <a href={`#`} class="nav-link"><i class="fa-brands fa-upwork"></i></a>
      </li>
    </ul>
  </section>
  <section class="header">
    <ul class="header-social-links">
      <li class="social-item">
        <a href={`#`} class="social-link"><i class="fa-brands fa-github"></i></a
        >
      </li>
      <li class="social-item">
        <a href={`#`} class="social-link"
          ><i class="fa-brands fa-telegram blue"></i></a
        >
      </li>
      <li class="social-item">
        <a href={`#`} class="social-link"
          ><i class="fa-regular fa-envelope red"></i></a
        >
      </li>
    </ul>
    <div class="header-content-container">
      <h1 class="header-content-header">
        Hi <span class="header-content-header">I am Daniel E.</span>
      </h1>

      <p class="header-content">
        Experienced Full-stack Developer with 3+ years experience,
        <span class="header-content">
          specialized in MERN stack (<span class="blue">React</span>,
          <span class="green">Node.js</span>,
          <span>Express</span>,
          <span class="green">MongoDB</span>...)
        </span>
      </p>
      <button class="header-btn">Download CV</button>
    </div>
    <div class="header-img-container">
      <img src={Logo} alt="computer guy" class="header-img-logo" />
    </div>
    <!-- <ul class="header-social-links">
      <li class="social-item">
        <a href={`#`} class="social-link"><i class="fa-brands fa-github"></i></a
        >
      </li>
      <li class="social-item">
        <a href={`#`} class="social-link"
          ><i class="fa-brands fa-telegram blue"></i></a
        >
      </li>
      <li class="social-item">
        <a href={`#`} class="social-link"
          ><i class="fa-regular fa-envelope red"></i></a
        >
      </li>
    </ul> -->
  </section>
</main>

<style>
  .main {
    display: flex;
    flex-direction: column;
    gap: 4rem;
  }
  .blue {
    color: #387adf;
  }
  .green {
    color: #65b741;
  }
  .red {
    color: #ff004d;
  }
  .navbar {
    padding: 2rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
  }
  .nav {
    display: flex;
    list-style-type: none;
    gap: 3rem;
  }
  .nav-link {
    font-weight: 600;
  }
  .navbar-social-links .nav-link {
    font-size: 1.2rem;
  }
  .logo {
    font-size: 1.7rem;
    font-weight: 700;
  }
  .fa-upwork {
    color: #65b741 !important;
  }
  .fa-linkedin-in {
    color: #387adf !important;
  }
  .header {
    padding: 4rem 2rem;
    display: flex;
    gap: 2rem;
    align-items: center;
    justify-content: space-between;
  }

  .header-content-header {
    display: block;
    font-size: 3rem;
  }
  .header-content-container {
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }
  .header-content {
    display: block;
    margin: 0.5rem 0;
  }
  .header-btn {
    border: 2px solid #ffff;
    padding: 0.7rem;
    background: inherit;
    color: #ffff;

    max-width: 150px;
    cursor: pointer;
  }

  .header-social-links {
    list-style-type: none;
    display: flex;
    flex-direction: column;
    gap: 2rem;
  }
  .social-link {
    font-size: 1.2rem;
  }
  .header-img-logo {
    border-radius: 50%;

    max-width: 300px;
    height: 300px;
  }
</style>
