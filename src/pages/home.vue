<template>
  <div>
    <div>
      <nav
        class="navbar is-fixed-top"
        role="navigation"
        aria-label="main navigation"
      >
        <div class="navbar-brand">
          <a
            class="navbar-item"
            href="#home"
            v-smooth-scroll="{ duration: 1000, offset: -50 }"
          >
            Amaka Eguzoro
          </a>

          <a
            role="button"
            class="navbar-burger burger"
            aria-label="menu"
            aria-expanded="false"
            data-target="navbarBasicExample"
            :class="{ 'is-active': showNav }"
            @click="showNav = !showNav"
          >
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div class="navbar-end">
          <a
            href="#home"
            v-smooth-scroll="{ duration: 2000, offset: -50 }"
            class="navbar-item"
          >
            Home
          </a>
          <a
            href="#contact"
            v-smooth-scroll="{ duration: 2000, offset: -50 }"
            class="navbar-item"
          >
            Contact
          </a>
          <a
            href="#projects"
            v-smooth-scroll="{ duration: 2000, offset: -50 }"
            class="navbar-item"
          >
            Projects
          </a>
          <!-- <router-link to="/contact" class="navbar-item">
           Contact
          </router-link> -->
        </div>
      </nav>
    </div>
    <!-- body -->
    <body>
      <div class="statement">
        <div class="introduction col-md-6">
          <p class="welcome">Hello I'm</p>
          <h1 class="my-name">Eguzoro Chimamaka</h1>
          <p class="occupation">Frontend Developer</p>
          
        </div>
        <router-view/>
      </div>

      <div class="total-body">
        <div class="card about-me">
          <!-- card navbar -->
          <nav class="navbar navbar-expand-lg card-navbar ">
            <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav">
                <li class="nav-item ">
                  <a class="nav-link" href="#">About</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Skills</a>
                </li>
                <li class="nav-item">
                  <a class="nav-link" href="#">Resume</a>
                </li>
              </ul>
            </div>
          </nav>

          <div class="card-body">
              <about />
              <skills/>
              <resume />
          </div>
        </div>
        <div>
        <projects />
      </div>
      <br>
      <br>

      <contacts />

      <br>

       <footer class="footer " >
      <p class="footer-text">
        Built by Chimamaka Eguzoro with Vue JS
      </p>
  
  </footer>

      </div>

      
    </body>
  </div>
</template>

<script>
import about from "../pages/about.vue"
import Resume from './resume.vue';
import Skills from './skills.vue';
import projects from './projects.vue'
import Contacts from './contacts.vue';

export default {
  components: {
      about,
    Resume,
    Skills,
    projects,
    Contacts
  }
};
</script>

<style scoped>
.navbar {
  background-color: #630a10;
}

.navbar-item {
  margin: 20px;
  color: #e1c699;
  text-decoration: none;
}
.statement {
  background-image: url("../assets/ama-background.png");
  height: 550px;
}
.introduction {
  padding: 100px;
  height: 400px;
  width: 400px;
}
.welcome {
  font-family: "Times New Roman";
  font-size: 40px;
  color: #e1c699;
}

.my-name {
  font-family: "Arial Black";
  font-size: 60px;
  color: #fff;
}

.occupation {
  font-family: "Times New Roman";
  font-size: 24px;
  color: #fff;
}

.about-me {
  background-color: #911f27;
  width: 90%;
  margin-left: 60px;
  margin-right: 30px;
}
.total-body {
  background-color: #630a10;
}

.card-navbar {
  background-color: #e1c699;
}
.nav-link {
  margin-left: 40px;
  margin-right: 30px;
  font-family: "Tahoma";
  color: black;
  text-decoration: none;
}
a:hover,
a:active {
  background-color: #630a10;
  color: white;
  text-decoration: none;
}

.footer-text{
  color: #e1c699;
  font-family: "Times New Roman";
  font-size: 15px;
  text-align: center;
}


</style>
