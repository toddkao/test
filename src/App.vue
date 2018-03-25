<template>
  <div id="app">
    <b-navbar variant="dark" type="white" id="navbar" toggleable>
      <b-navbar-brand href="#">
        <img src="https://material.io/guidelines/static/spec/images/callouts/default.svg" width="50px" height="50px">
        Test Site
      </b-navbar-brand>
      <b-navbar-nav>
        <b-nav-item>LINK1</b-nav-item>
        <b-nav-item>LINK2</b-nav-item>
        <b-nav-item>LINK3</b-nav-item>
        <b-nav-item>LINK4</b-nav-item>
      </b-navbar-nav>
    </b-navbar>
    <router-view/>
    <footer>
      <b-container class="footer-container">
          <b-row>
            <b-col>
              <ul>
                <li>Some company inc</li>
                <li><img src="@/assets/logo.png" width="50px" height="50px"></li>
              </ul>
            </b-col>
            <b-col>
              <ul>
                <li><a href="/">LINKS1</a></li>
                <li><a href="/">LINKS2</a></li>
                <li><a href="/">LINKS3</a></li>
                <li><a href="/">LINKS4</a></li>
              </ul>
            </b-col>
            <b-col>
              <ul>
                <li><a href="/">LINKS5</a></li>
                <li><a href="/">LINKS6</a></li>
                <li><a href="/">LINKS7</a></li>
                <li><a href="/">LINKS8</a></li>
              </ul>
            </b-col>
            <b-col>
              <ul>
                <li>SOCIAL MEDIA</li>
              </ul>
            </b-col>
          </b-row>
      </b-container>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      msg: [1, 2, 3, 4, 5]
    }
  },
  mounted () {},
  methods: {
    test () {
      console.log('LOG')
      console.log(
        this.msg.map((x, i) => {
          return x + 1
        })
      )
    }
  }
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: auto
}
#navbar{
  text-align: center;
  margin: auto
}
footer{
  background: #343a40;
  color: antiquewhite
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  margin: 10px 10px;
}
</style>
