<script>
  const navLinks = ["Home", "Aboutme", "Showcase"];
</script>

<section class="navbar">
  <a class="logo" href={``}>D.E</a>
  <ul class="nav">
    {#each navLinks as links (links)}
      <li class="nav-item">
        <a href={`#${links}`} class="nav-link">{links}</a>
      </li>
    {/each}
  </ul>
  <ul class="nav navbar-social-links">
    <li class="nav-item">
      <a href={`#`} class="nav-link"><i class="fa-brands fa-linkedin-in"></i></a
      >
    </li>
    <li class="nav-item">
      <a href={`#`} class="nav-link"><i class="fa-brands fa-upwork"></i></a>
    </li>
  </ul>
</section>
<section class="header">
  <div class="header-content-container">
    <h1 class="header-content-header">Hi i am Daniel E.</h1>
    <p class="header-content"></p>
  </div>
  <div class="header-img-container"></div>
</section>

<style>
  .navbar {
    padding: 1rem 2rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
  }
  .nav {
    display: flex;
    list-style-type: none;
    gap: 3rem;
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
</style>
