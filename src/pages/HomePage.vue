<template>
  <div class="container-fluid bg-black">

<!-- SECTION HOME -->
    <section id="home">
      <div class="background-img">
        <div class="row">
          <div class="mt-4 text-end">
            <!-- <GlowingIcons /> -->
          </div>
        </div>
    
<!-- STUB DESKTOP VIEW -->
        <div class="row mb-5">
          <div class="col-md-6 col-12 m-auto mt-5 me-5 pt-5 heading-section">
            <div class="mt-5 ms-2 text-black typewriter pt-5 d-md-block d-none">
              <h1 class="fs-5 mt-5 text-shadow">Hi, I'm Andrew</h1>
                <h1 class="fs-5 text-shadow">A full-stack <span class="fs-1 text-info">Software Developer</span></h1>
            </div>

<!-- STUB MOBILE VIEW -->
            <div class="mt-5 ms-2 text-black text-center pt-1 d-block d-md-none">
              <h1 class="fs-5 mt-5 text-shadow">Hi, I'm Andrew</h1>
                <h1 class="fs-5 text-shadow">A full-stack</h1>
                <h1 class="text-info">Software Developer</h1>
            </div>

          </div>
        </div>
      </div>
    </section>


<!-- SECTION ABOUT -->
    <section id="about" class="about py-1">
      <AboutComponent />
      <SkillsComponent />
    </section>


<!-- SECTION APPLICATIONS -->
<section id="applications" class="applications">
  <div class="background-third">
    <div class="row">
      <div class="col-md-8 col-12 app-heading">
        <h2 class="fs-1 app-text text-center">Applications</h2>
      </div>
    </div>

<!-- NOTE have it cycle through multiple imgs of apps here would be cool -->

<!-- STUB DEVS AND DRAGONS INFO -->
    <DDAppComponent />

    <div class="row">
      <div class="col-12 app-line-break">
        <div class="full-h-line"></div>
      </div>
    </div>
    
    
    <!-- STUB KEEPR INFO -->
    <KeeprComponent />



        <div class="row">
          <div class="col-12 app-line-break">
            <div class="full-h-line"></div>
          </div>
        </div>


<!-- STUB ALLSPICE INFO -->
        <AllSpiceComponent />

        <div class="row">
          <div class="col-12 app-line-break">
            <div class="full-h-line"></div>
          </div>
        </div>
  </div>
</section>

    <!-- SECTION FORM -->
<section id="contact" class="contact">
  <ContactComponent />
</section>

  </div>
</template>

<script>
import ContactComponent from "../components/ContactComponent.vue";

// import assets from "scr/assets/img";



export default {
    setup() {
        return {

        };
    },
    components: { ContactComponent }
}
</script>

<style scoped lang="scss">

.background-img{
  background-image: url('https://static.vecteezy.com/system/resources/previews/002/821/966/original/abstract-triangular-geometric-background-free-vector.jpg');
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
}
.text-shadow{
  text-shadow: 1px 1px gray;
}
.background-third {
  background: rgb(20,182,197);
background: linear-gradient(90deg, rgba(20,182,197,1) 0%, rgba(8,56,72,1) 50%, rgba(20,86,96,1) 100%);
}
.app-heading{
  margin-top: 3rem;
  margin-bottom: 3rem;
  margin-left: auto;
  margin-right: auto;
  padding-top: 1.5rem;
}

.full-h-line {
  height: 1px;
  width: 100%;
  background: white;
}

.app-text{
  color: #f7a51b;
}
.app-line-break{
  margin-top: 3rem;
  margin-bottom: 3rem;
}

.typewriter h1 {
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: .15em solid orange; /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: .15em; /* Adjust as needed */
  animation: 
    typing 3.5s steps(40, end),
    blink-caret .75s step-end infinite;
}

/* The typing effect */
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

/* The typewriter cursor effect */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}

@media screen and (max-width: 769px) {
  
  .heading-section{
    margin-left: 0px;
  }
  .app-heading{
  margin-top: 1rem;
  margin-bottom: 1rem;
  margin-left: auto;
  margin-right: auto;
  padding-top: 1rem;
}
.app-line-break{
  margin-top: 1rem;
  margin-bottom: 1rem;
}
  .vue-icon{
    height: 5em;
    padding: 4px;
  }
  .node-icon{
    height: 5em;
    padding: 4px;
  }
  .mongo-icon{
    height: 5em;
    padding: 4px;
  }
  .post-icon{
    height: 5em;
    padding: 4px;
  }
  .dd-icon-section{
    margin-left: 1rem;
    margin-right: 1rem;
    
  }






.typewriter h1 {
  
  overflow: none; /* Ensures the content is not revealed until the animation */
  border-right: none; /* The typwriter cursor */
  white-space: wrap; /* Keeps the content on a single line */
  margin: 0 auto; /* Gives that scrolling effect as the typing happens */
  margin-left: 3rem;
  letter-spacing: .10em; /* Adjust as needed */
  animation: 
    none;
}
@keyframes typing {
  from { width: 0 }
  to { width: 100% }
}

}




</style>
