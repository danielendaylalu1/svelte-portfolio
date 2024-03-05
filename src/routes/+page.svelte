<script lang="ts">
  // import { LOOP } from "@splidejs/splide";
  import Logo from "../asset/profile.png";
  import Navbar from "../components/Navbar.svelte";
  import "../style/index.css";
  import Express from "../asset/logos/express.svg";
  import React from "../asset/logos/react.svg";
  import Nodejs from "../asset/logos/node-js.svg";
  import Css from "../asset/logos/css.svg";
  import Html from "../asset/logos/html.svg";
  import Mongodb from "../asset/logos/mongodb.svg";
  import Bootstrap from "../asset/logos/bootstrap.svg";
  import Redux from "../asset/logos/redux.svg";
  import Javascript from "../asset/logos/javascript.svg";
  import Tailwind from "../asset/logos/tailwind-css.svg";
  import Sql from "../asset/logos/sql.svg";
  import Nextjs from "../asset/logos/nextjs.png";
  import Svelte from "../asset/logos/svelte.png";
  import Frontend from "../asset/gifs/frontend.png";
  import Backend from "../asset/gifs/backend.png";
  import Database from "../asset/gifs/database.png";
  import Gsap from "../asset/logos/gsap.svg";

  import Onship from "../asset/images/onship.png";
  import MusicExplore from "../asset/images/music-explore.png";

  let logos = [
    Html,
    Css,
    Bootstrap,
    Tailwind,
    Javascript,
    React,
    Nextjs,
    Svelte,
    Redux,
    Nodejs,
    Express,
    Mongodb,
    Sql,
  ];
</script>

<main class="main">
  <Navbar />
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
  </section>
  <section class="about" id="Aboutme">
    <h1 class="about-header t-center">About Me</h1>

    <p class="about-content">
      I am an experienced Full-stack Developer with a proven track record in
      developing high-quality websites and web applications. My expertise lies
      in developing attractive , dynamic and functional website using the latest
      web frameworks and libraries.
    </p>
    <p class="about-content">
      My projects involve seamless API integration for enhanced functionalities,
      pixel perfect design conversion, clean and optimize written codes.I adhere
      to Agile methodologies, ensuring an adaptive, flexible, and
      result-oriented approach in every project I undertake.
    </p>
  </section>
  <section class="skills">
    <h2 class="header-small t-center">Skills</h2>
    <div class="skills-logo-container">
      {#each logos as logo, index (index)}
        <img src={logo} alt="logo" class="skills-img" />
      {/each}
    </div>
  </section>
  <section class="services">
    <h2 class="header-small t-center">Services I Offer</h2>
    <div class="services-card-container">
      <div class="services-card">
        <img src={Frontend} alt="frontend gif" />
        <h3 class="card-title">Frontend Development</h3>
        <p class="card-content">
          Build Responsive, Attractive, Dynamic and interactive Websites.
          Transform designs into functional and accessible interfaces.
        </p>
      </div>
      <div class="services-card">
        <img src={Backend} alt="frontend gif" />
        <h3 class="card-title">Backend Development</h3>
        <p class="card-content">
          Build server-side logic of a web applications. create, maintain, and
          optimize servers and databases that power the user-facing side of a
          website. Design and implement APIs
        </p>
      </div>
      <div class="services-card">
        <img src={Database} alt="frontend gif" />
        <h3 class="card-title">Database Management</h3>
        <p class="card-content">
          Design, implement, maintain, and repair an organization’s database.
          Create a performance, integrited , and well secured database. Store
          and organize data effectively
        </p>
      </div>
    </div>
  </section>
  <section class="projects" id="Showcase">
    <h2 class="header-small t-center">Recent Projects</h2>
    <div class="projects-card-container">
      <div class="projects-card">
        <img src={Onship} alt="onship project" />
        <div class="card-content-container">
          <h3 class="card-title">Ship On</h3>
          <p class="card-content">
            In publishing and graphic design, Lorem ipsum is a placeholder text
            commonly used to demonstrate the visual form of a document or a
            typeface without relying on meaningful content. Lorem ipsum may be
            used as a placeholder before the final copy is available.
          </p>
          <div class="card-skills">
            <img src={React} alt="" />
            <img src={Gsap} alt="" />
          </div>
          <div class="card-btns">
            <a href="#" class="card-btn"><i class="fa-brands fa-github"></i></a>
            <a href="#" class="blue">Link</a>
          </div>
        </div>
      </div>
      <div class="projects-card">
        <img src={MusicExplore} alt="onship project" />
        <div class="card-content-container">
          <h3 class="card-title">Music Explore</h3>
          <p class="card-content">
            In publishing and graphic design, Lorem ipsum is a placeholder text
            commonly used to demonstrate the visual form of a document or a
            typeface without relying on meaningful content. Lorem ipsum may be
            used as a placeholder before the final copy is available.
          </p>
          <div class="card-skills">
            <img src={React} alt="" />
            <img src={Express} alt="" />
            <img src={Mongodb} alt="" />
            <img src={Redux} alt="" />
          </div>
          <div class="card-btns">
            <a href="#" class="card-btn"><i class="fa-brands fa-github"></i></a>
            <a href="#" class="blue">Link</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</main>
