<template>
  <!-- Desktop Navigation -->
  <nav id="desktop-nav">
    <div class="logo">MSD</div>
    <div>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hamburger Navigation -->
  <nav id="hamburger-nav">
    <div class="logo">MSD</div>
    <div class="hamburger-menu">
      <div class="hamburger-icon" @click="toggleMenu" :class="{ open: isOpen }">
        <span></span>
        <span></span>
        <span></span>
      </div>
      <div :class="{ open: isOpen , 'menu-links':isOpen , 'menu-links-close': !isOpen }">
        <ul>
          <li><a href="#about" @click="toggleMenu">About</a></li>
          <li><a href="#experience" @click="toggleMenu">Experience</a></li>
          <li><a href="#projects" @click="toggleMenu">Projects</a></li>
          <li><a href="#contact" @click="toggleMenu">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>
  <section id="profile">
    <div class="section__pic-container">
      <img src="./assets/profile-pic.jpg" alt="MSD profile picture" />
    </div>
    <div class="section__text">
      <p class="section__text__p1">Hello, I'm</p>
      <h1 class="title">Mehmet Salih Durdu</h1>
      <p class="section__text__p2">Full Stack Website Developer</p>
      <p class="section__text__p2">Computer Engineer</p>
      <div class="btn-container">
        <button class="btn btn-color-2" onclick="window.open('https://bit.ly/mehmetsalihdurduCv', '_blank')">
          Download CV
        </button>
        <button class="btn btn-color-1" onclick="location.href='./#contact'">
          Contact Info
        </button>
      </div>
      <div id="socials-container">
        <img src="./assets/instagram.png" alt="My Instagram profile" class="icon"
          onclick="window.open('https://www.instagram.com/mehmetsdrd/', '_blank')" />
        <img src="./assets/linkedin.png" alt="My LinkedIn profile" class="icon"
          onclick="window.open('https://linkedin.com/in/mehmet-salih-durdu', '_blank')" />
        <img src="./assets/github.png" alt="My Github profile" class="icon"
          onclick="window.open('https://github.com/MarkM5D', '_blank')" />
      </div>
    </div>
  </section>
  <section id="about">
    <p class="section__text__p1">Get To Know More</p>
    <h1 class="title">About Me</h1>
    <div class="section-container">
      <div class="section__pic-container">
        <img src="./assets/about-pic.jpg" alt="Profile picture" class="about-pic" />
      </div>
      <div class="about-details-container">
        <div class="about-containers">
          <div class="details-container">
            <img src="./assets/experience.png" alt="Experience icon" class="icon" />
            <h3>Experience</h3>
            <p>half+ years <br />Full Stack Website Development</p>
          </div>
          <div class="details-container">
            <img src="./assets/education.png" alt="Education icon" class="icon" />
            <h3>Education</h3>
            <p>Bachelor's Degree<br />Computer Engineering</p>
          </div>
        </div>
        <div class="text-container">
          <p>
            I am a computer engineer and also a YouTuber. I have experience working on small projects in
            various
            programming languages such as C, C++, Java, ReactJS, Firebase, HTML, CSS, JS, MSSQL, ASP.NET MVC, Bootstrap,
            Flutter, VueJS, PHP, and Python API (NLP). Currently, I am actively focusing on full-stack web development
            using
            ReactJS
            and Firebase. In my free time, I enjoy creating "how-to" style videos for my YouTube channel.
          </p>
        </div>
      </div>
    </div>
    <img src="./assets/arrow.png" alt="Arrow icon" class="icon arrow" onclick="location.href='./#experience'" />
  </section>
  <section id="experience">
    <p class="section__text__p1">Explore My</p>
    <h1 class="title">Experience</h1>
    <div class="experience-details-container">
      <div class="about-containers">
        <div class="details-container">
          <h2 class="experience-sub-title">Frontend Development</h2>
          <div class="article-container">
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>HTML</h3>
                <p>Experienced</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>CSS</h3>
                <p>Experienced</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>REACTJS</h3>
                <p>Intermediate</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>JavaScript</h3>
                <p>Basic</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>BOOTSTRAP</h3>
                <p>Intermediate</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>VUEJS&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
                <p>Basic</p>
              </div>
            </article>
          </div>
        </div>
        <div class="details-container">
          <h2 class="experience-sub-title">Backend Development</h2>
          <div class="article-container">
            <article>
              <img src="./assets/checkmark.png" style="margin-left: 3px;" alt="Experience icon" class="icon" />
              <div>
                <h3>FIREBASE</h3>
                <p>Intermediate</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>MSSQL&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
                <p>Basic</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>JAVA&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
                <p>Basic</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>PHP&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
                <p>Basic</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>ASP.NET <br/>MVC &nbsp;&nbsp;</h3>
                <p>Intermediate</p>
              </div>
            </article>
            <article>
              <img src="./assets/checkmark.png" alt="Experience icon" class="icon" />
              <div>
                <h3>PYTHON&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</h3>
                <p>Basic</p>
              </div>
            </article>
          </div>
        </div>
      </div>
    </div>
    <img src="./assets/arrow.png" alt="Arrow icon" class="icon arrow" onclick="location.href='./#projects'" />
  </section>
  <section id="projects">
    <p class="section__text__p1">Browse My Recent</p>
    <h1 class="title">Projects</h1>
    <div class="experience-details-container">
      <div class="about-containers">
        <div class="details-container color-container">
          <div class="article-container">
            <img src="./assets/ustavar.png" alt="Ustavar" class="project-img" />
          </div>
          <h2 class="experience-sub-title project-title">USTAVAR</h2>
          <div class="btn-container">
            <button class="btn btn-color-2 project-btn" onclick="window.open('https://ustavar.com.tr', '_blank')">
              Visit the website
            </button>
          </div>
        </div>
        <div class="details-container color-container">
          <div class="article-container">
            <img src="./assets/onasor.png" alt="Onasor" class="project-img" />
          </div>
          <h2 class="experience-sub-title project-title">ONASOR</h2>
          <div class="btn-container">
            <button class="btn btn-color-2 project-btn" onclick="return false;">
              Developing
            </button>
          </div>
        </div>
        <div class="details-container color-container">
          <div class="article-container">
            <img src="./assets/cilginmsd.png" alt="CilginMSD" class="project-img" />
          </div>
          <h2 class="experience-sub-title project-title">Çılgın MSD</h2>
          <div class="btn-container">
            <button class="btn btn-color-2 project-btn"
              onclick="window.open('https://www.youtube.com/@CILGINMSD', '_blank')">
              Youtube Channel
            </button>
          </div>
        </div>
      </div>
    </div>
    <img src="./assets/arrow.png" alt="Arrow icon" class="icon arrow" onclick="location.href='./#contact'" />
  </section>
  <section id="contact">
    <p class="section__text__p1">Get in Touch</p>
    <h1 class="title">Contact Me</h1>
    <div class="contact-info-upper-container">
      <div class="contact-info-container">
        <img src="./assets/email.png" alt="Email icon" class="icon contact-icon email-icon" />
        <p><a href="mailto:mehmetsalihd20@gmail.com">mehmetsalihd20@gmail.com</a></p>
      </div>
      <div class="contact-info-container">
        <img src="./assets/linkedin.png" alt="LinkedIn icon" class="icon contact-icon" />
        <p><a href="https://www.linkedin.com/in/mehmet-salih-durdu" target="_blank">LinkedIn</a></p>
        <img src="./assets/instagram.png" alt="LinkedIn icon" class="icon contact-icon" />
        <p><a href="https://www.instagram.com/mehmetsdrd/" target="_blank">Instagram</a></p>
      </div>
    </div>
  </section>
  <footer>
    <nav>
      <div class="nav-links-container">
        <ul class="nav-links">
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>
    <p>Copyright &#169; 2023 Mehmet Salih Durdu. All Rights Reserved.</p>
  </footer>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      isOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isOpen = !this.isOpen;
    }
  }
};
</script>

<style>
/* GENERAL */

@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&display=swap");

* {
  margin: 0;
  padding: 0;
}

body {
  font-family: "Poppins", sans-serif;
}

html {
  scroll-behavior: smooth;
}

p {
  color: rgb(85, 85, 85);
}

/* TRANSITION */

a,
.btn {
  transition: all 300ms ease;
}

/* DESKTOP NAV */

nav,
.nav-links {
  display: flex;
}

nav {
  justify-content: space-around;
  align-items: center;
  height: 17vh;
}

.nav-links {
  gap: 2rem;
  list-style: none;
  font-size: 1.5rem;
}

a {
  color: black;
  text-decoration: none;
  text-decoration-color: white;
}

a:hover {
  color: grey;
  text-decoration: underline;
  text-underline-offset: 1rem;
  text-decoration-color: rgb(181, 181, 181);
}

.logo {
  font-size: 2rem;
}

.logo:hover {
  cursor: default;
}

/* HAMBURGER MENU */

#hamburger-nav {
  display: none;
}

.hamburger-menu {
  position: relative;
}

.hamburger-icon {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 24px;
  width: 30px;
  cursor: pointer;
}

.hamburger-icon span {
  width: 100%;
  height: 2px;
  background-color: black;
  transition: all 0.3 ease-in-out;
}

.menu-links {
  position: absolute;
  top: 100%;
  right: 0;
  background-color: rgb(252, 252, 252);
  width: fit-content;
  max-height: 0;
  overflow: hidden;
  transition: all 0.3 ease-in-out;
  display: inline-block;
  border-radius: 13px;
  margin-top: 5px;
  border: 0.5px solid gray;
  border-bottom: 0;
}
.menu-links-close{
  display: none;
}

.menu-links a {
  display: block;
  padding: 10px;
  text-align: center;
  font-size: 1.5rem;
  color: black;
  text-decoration: none;
  transition: all 0.3 ease-in-out;
  border-bottom: 0.3px solid gray;
}

.menu-links li {
  list-style: none;
}

.menu-links.open {
  max-height: 300px;
}

.hamburger-icon.open span:first-child {
  transform: rotate(45deg) translate(10px, 5px);
}

.hamburger-icon.open span:nth-child(2) {
  opacity: 0;
}

.hamburger-icon.open span:last-child {
  transform: rotate(-45deg) translate(10px, -5px);
}

.hamburger-icon span:first-child {
  transform: none;
}

.hamburger-icon span:first-child {
  opacity: 1;
}

.hamburger-icon span:first-child {
  transform: none;
}

/* SECTIONS */

section {
  padding-top: 4vh;
  height: 96vh;
  margin: 0 10rem;
  box-sizing: border-box;
  min-height: fit-content;
}

.section-container {
  display: flex;
}

/* PROFILE SECTION */

#profile {
  display: flex;
  justify-content: center;
  gap: 5rem;
  height: 80vh;
}

.section__pic-container {
  display: flex;
  height: 400px;
  width: 400px;
  margin: auto 0;
}

.section__text {
  align-self: center;
  text-align: center;
}

.section__text p {
  font-weight: 600;
}

.section__text__p1 {
  text-align: center;
}

.section__text__p2 {
  font-size: 1.75rem;
  margin-bottom: 1rem;
}

.title {
  font-size: 3rem;
  text-align: center;
}

#socials-container {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 1rem;
}

/* ICONS */

.icon {
  cursor: pointer;
  height: 2rem;
}

/* BUTTONS */

.btn-container {
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.btn {
  font-weight: 600;
  transition: all 300ms ease;
  padding: 1rem;
  width: 18.3rem;
  border-radius: 18px;
}

.btn-color-1,
.btn-color-2 {
  border: rgb(53, 53, 53) 0.1rem solid;
}

.btn-color-1:hover,
.btn-color-2:hover {
  cursor: pointer;
}

.btn-color-1,
.btn-color-2:hover {
  background: rgb(53, 53, 53);
  color: white;
}

.btn-color-1:hover {
  background: rgb(0, 0, 0);
}

.btn-color-2 {
  background: none;
}

.btn-color-2:hover {
  border: rgb(255, 255, 255) 0.1rem solid;
}

.btn-container {
  gap: 1rem;
}

/* ABOUT SECTION */

#about {
  position: relative;
}

.about-containers {
  gap: 2rem;
  margin-bottom: 2rem;
  margin-top: 2rem;
}

.about-details-container {
  justify-content: center;
  flex-direction: column;
}

.about-containers,
.about-details-container {
  display: flex;
}

.about-pic {
  border-radius: 2rem;
}

.arrow {
  position: absolute;
  right: -5rem;
  bottom: 2.5rem;
}

.details-container {
  padding: 1.5rem;
  flex: 1;
  background: white;
  border-radius: 18px;
  border: rgb(53, 53, 53) 0.1rem solid;
  border-color: rgb(163, 163, 163);
  text-align: center;
}

.section-container {
  gap: 4rem;
  height: 80%;
}

.section__pic-container {
  height: 400px;
  width: 400px;
  margin: auto 0;
}

/* EXPERIENCE SECTION */

#experience {
  position: relative;
}

.experience-sub-title {
  color: rgb(85, 85, 85);
  font-weight: 600;
  font-size: 1.75rem;
  margin-bottom: 2rem;
}

.experience-details-container {
  display: flex;
  justify-content: center;
  flex-direction: column;
}

.article-container {
  display: flex;
  text-align: initial;
  flex-wrap: wrap;
  flex-direction: row;
  gap: 2.5rem;
  justify-content: space-around;
}

article {
  display: flex;
  width: 10rem;
  justify-content: space-around;
  gap: 0.5rem;
}

article .icon {
  cursor: default;
}

/* PROJECTS SECTION */

#projects {
  position: relative;
}

.color-container {
  border-color: rgb(163, 163, 163);
  background: rgb(250, 250, 250);
}

.project-img {
  border-radius: 13px;
  width: 90%;
  height: 90%;
}

.project-title {
  margin: 1rem;
  color: black;
}

.project-btn {
  color: black;
  border-color: rgb(163, 163, 163);
}

/* CONTACT */

#contact {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 70vh;
}

.contact-info-upper-container {
  display: flex;
  justify-content: center;
  border-radius: 2rem;
  border: rgb(53, 53, 53) 0.1rem solid;
  border-color: rgb(163, 163, 163);
  background: (250, 250, 250);
  margin: 2rem auto;
  padding: 0.5rem;
}

.contact-info-container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  margin: 1rem;
}

.contact-info-container p {
  font-size: larger;
}

.contact-icon {
  cursor: default;
}

.email-icon {
  height: 2.5rem;
}

/* FOOTER SECTION */

footer {
  height: 26vh;
  margin: 0 1rem;
}

footer p {
  text-align: center;
}

@media screen and (max-width: 1400px) {
  #profile {
    height: 83vh;
    margin-bottom: 6rem;
  }

  .about-containers {
    flex-wrap: wrap;
  }
}

@media screen and (max-width: 1200px) {
  #desktop-nav {
    display: none;
  }

  #hamburger-nav {
    display: flex;
  }

  #experience,
  .experience-details-container {
    margin-top: 2rem;
  }

  #profile,
  .section-container {
    display: block;
  }

  .arrow {
    display: none;
  }

  section,
  .section-container {
    height: fit-content;
  }

  section {
    margin: 0 5%;
  }

  .section__pic-container {
    width: 275px;
    height: 275px;
    margin: 0 auto 2rem;
  }

  .about-containers {
    margin-top: 0;
  }
}

@media screen and (max-width: 600px) {

  #contact,
  footer {
    height: 40vh;
  }

  #profile {
    height: 83vh;
    margin-bottom: 0;
  }

  article {
    font-size: 1rem;
  }

  footer nav {
    height: fit-content;
    margin-bottom: 2rem;
  }

  .about-containers,
  .contact-info-upper-container,
  .btn-container {
    flex-wrap: wrap;
  }

  .contact-info-container {
    margin: 0;
  }

  .contact-info-container p,
  .nav-links li a {
    font-size: 1rem;
  }

  .experience-sub-title {
    font-size: 1.25rem;
  }

  .logo {
    font-size: 1.5rem;
  }

  .nav-links {
    flex-direction: column;
    gap: 0.5rem;
    text-align: center;
  }

  .section__pic-container {
    width: auto;
    height: 46vw;
    justify-content: center;
  }

  .section__text__p2 {
    font-size: 1.25rem;
  }

  .title {
    font-size: 2rem;
  }

  .text-container {
    text-align: justify;
  }
}
</style>
