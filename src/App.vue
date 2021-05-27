<template>
  <div id="app">
    <Navbar />
    <div class="home">
      <div class="container">
        <div class="row">
          <div class="col text-center header">
            <h1>{ Hello, World }</h1>
          </div>
        </div>
        <main>
          <div class="row">
            <div class="col">
              <div class="about">
                <div class="row">
                  <div class="col">
                    <h4>Christopher Arias</h4>
                    <a href="mailto:christopher.arias.jr@gmail.com">Christopher.arias.jr@gmail.com</a>
                  </div>
                  <div class="col text-right">
                    <h5 style="position: absolute; bottom: -11px; right: 18px;">Web-Developer</h5>
                  </div>
                </div>
                <hr />
                <span>
                  Born and raised in Arizona. Loves to code and develop software. Quick and effecient. Works well with people. Coffee might be accepted as a form of payment. 
                </span>
              </div>
              <div class="social">
                <h4>Social Sites</h4>
                <hr>
                <ul>
                  <li><a href="https://github.com/christopherariasjr">Github</a></li>
                  <li><a href="https://www.linkedin.com/in/christopher-arias-66b959176/">Linkedin</a></li>
                </ul>
              </div>
              <div class="projects">
                <h4>Projects</h4>
                <hr>
                <ul class v-for="item in projects" :key="item.name">
                  <li>{{item.name}} - <a :href="item.url">{{item.url}}</a></li>
                </ul>
              </div> 
            </div>
          </div>
        </main>
      </div>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar'

export default {
  components: {
    Navbar
  },  
  data: () => {
    return {
      projects: [
        {
          url: "http://bitwatcher.ariaslabs.com",
          name: "Bitwatcher"
        },
        {
          url: "https://weathertrack.ariaslabs.com",
          name: "Weathertrack"
        }
      ]
    }
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Share+Tech&family=Share+Tech+Mono&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Share Tech', sans-serif;
  background: rgb(49, 49, 49);
  color: white;
}


  h1, h2, h3, h4 h5, h6 {
    font-family: 'Share Tech Mono', monospace;
  }

  .home {
    margin-top: 14em;
  }

  main {
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    padding-left: 10px;
    margin-bottom: 5em;
  }

  .header {
    padding-left: 20px !important;
  }

  .about {
    position: relative;
    margin-top: 18em;
    
  }

  .social {
    margin-top: 5em;
  }

  .projects {
    margin-top: 5em;
  }

  hr {
    color: white !important ;
    background:  white;
  }

  a {
     color: white !important;
     text-decoration: underline !important;
  }

  a:hover {
    color: rgb(255, 216, 87) !important;
  }

  ul {
    list-style-type: none;
  }
</style>
