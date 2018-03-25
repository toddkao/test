<template>
  <div class="hello">
    <!--h1>{{ msg }}</h1-->
    <b-carousel id="carousel1"
                style="text-shadow: 1px 1px 2px #333;"
                controls
                indicators
                background="#ababab"
                :interval="4000"
                img-width="1024"
                img-height="480"
                v-model="slide"
    >

      <b-carousel-slide img-blank
                        content-tag="div">
        <div class="item">
          <b-jumbotron header="Jumbotron" lead="Jumbotron in carousel test" >
            <h5>Some info</h5>
            <p>More info</p>
            <b-btn variant="primary" href="#">A button</b-btn>
          </b-jumbotron>
          </div>
      </b-carousel-slide>
      <!-- Text slides with image -->
      <b-carousel-slide caption="First slide"
                        text="Nulla vitae elit libero, a pharetra augue mollis interdum."
                        img-src="https://lorempixel.com/1024/480/technics/2/"
      ></b-carousel-slide>

      <!-- Slides with custom text -->
      <b-carousel-slide img-src="https://lorempixel.com/1024/480/technics/4/">
        <h1>Hello world!</h1>
      </b-carousel-slide>

      <!-- Slides with image only -->
      <b-carousel-slide img-src="https://lorempixel.com/1024/480/technics/8/">
      </b-carousel-slide>

      <!-- Slides with img slot -->
      <!-- Note the classes .d-block and .img-fluid to prevent browser default image alignment -->
      <b-carousel-slide>
        <img slot="img" class="d-block img-fluid w-100" width="1024" height="480"
             src="https://lorempixel.com/1024/480/technics/5/" alt="image slot">
      </b-carousel-slide>

      <!-- Slide with blank fluid image to maintain slide aspect ratio -->
      <b-carousel-slide caption="Blank Image" img-blank img-alt="Blank image">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse
          eros felis, tincidunt a tincidunt eget, convallis vel est. Ut pellentesque
          ut lacus vel interdum.
        </p>
      </b-carousel-slide>

    </b-carousel>
    <b-container class="news">
      <b-row>
        <b-col>
          <h2>News</h2>
        </b-col>
      </b-row>
      <b-row>
        <b-col>
            <b-card title="News Article 1"
            img-src="https://lorempixel.com/600/300/food/5/"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 20rem;"
            class="mb-2">
            <p class="card-text">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
            </b-card>
        </b-col>
        <b-col>
          <b-card title="News Article 2"
            img-src="https://lorempixel.com/600/300/food/5/"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 20rem;"
            class="mb-2">
            <p class="card-text">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
            </b-card>
        </b-col>
        <b-col>
          <b-card title="News Article 3"
            img-src="https://lorempixel.com/600/300/food/5/"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 20rem;"
            class="mb-2">
            <p class="card-text">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
            <b-button href="#" variant="primary">Go somewhere</b-button>
            </b-card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#carousel1{
  width: 1024px;
  height: 480px;
  margin: auto
}
#hello{
  text-align: center;
  margin: auto
}
</style>
