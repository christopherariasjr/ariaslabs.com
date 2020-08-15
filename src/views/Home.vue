<template>
  <div class="home">
    <div class="container">
      <div class="row">
        <div class="col text-center">
          <h1>Hello World.</h1>
        </div>
      </div>
      <main>
        <div class="row">
          <div class="col">
            <div class="about">
              <h4>Christopher Arias</h4>
              <h5>Web-Developer</h5>
              <hr />
              <span>
                Born and raised in Arizona. Loves to code and develop software. Quick and effecient. Works well with people. Coffee might be used as a form of payment. 
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
              <ul>

              </ul>
            </div> 
          </div>
        </div>
      </main>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  components: {

  }
}
</script>

<style lang="scss" scoped>
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
    color: white !important;
    background:  white;
  }

  a {
     color: white;
     text-decoration: underline
  }

  ul {
    list-style-type: none;
  }
</style>