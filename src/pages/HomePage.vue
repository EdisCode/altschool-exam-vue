<template>
  <NavBar/>
  <section>
    <div className="avatar-container">
      <img width="100" height="120" src="../assets/picture.jpg" className="avatar" alt="avatar" title="avatar" loading="eager" />
      <h1 className="intro">Hi there! My name is Edikan Ekanem.</h1>
    </div>
    <div className="info">
      <h2>Nice of you to join me here.</h2>
      <p>
        Kindly check out my amazing Counter app I created using VUEJS.
      </p>
      <p>You can know more about me by clicking my name below. </p>
    </div>
  </section>
  <Footer/>
</template>

<script>
import { NavBar, Footer } from "../components";

export default {
  name: 'HomePage',
  components: {
    NavBar, Footer
  },
}
</script>