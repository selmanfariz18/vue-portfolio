<template>
  <v-app id="home">
    <NavBar />
    <v-container fluid>
      <div class="head">
        <v-row>
          <v-col cols="5">
            <div style="position: relative" class="mt-16">
            <h1 class="text-grey">Hello,</h1>
            <h1 class="text-white">I M SELMANUL FARIZY KA</h1>
            <span class="text-grey">Vue developer</span><br/>
            <v-btn tile dark class="text-red mt-8" variant="outlined">Contact Me</v-btn>
          </div>
          </v-col>
          <v-col cols="2">
            <div style="position:absolute;z-index: 9999;bottom:0;margin-left: auto;margin-right: auto;left:0;right: 0;text-align:center ;">
              <v-icon>fas fa-angle-double-down</v-icon>
            </div>
          </v-col>
          <v-col clos="5">
            <div style="position: relative;z-index: 9999;" class="mt-16">
              <v-img src="../../public/mine.png" contain max-height="300"></v-img>
            </div>
          </v-col>
        </v-row>
      </div>
      <v-col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="../../public/mine.png" max-height="300"></v-img>
              </div>
            </v-col>
            <v-col cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <div style="width:120px">
              <v-slider v-model="slider2" color="red" :label="track-color"></v-slider>
              </div>
              <h4 class="mt-n4">I am a Vue developer</h4>
              <h4>and Python programmer</h4>
              <p class="text-grey">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi, reiciendis? Aspernatur, nobis provident. Nulla aspernatur at similique repellat! Unde fugiat ipsum quod aliquid, dolores quibusdam nihil sit molestias quasi. Non?
              </p>
              <br/>
              <p class="text-grey">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eligendi, reiciendis? Aspernatur, nobis provident. Nulla aspernatur at similique repellat! Unde fugiat ipsum quod aliquid, dolores quibusdam nihil sit molestias quasi. Non?
              </p>
              <v-btn tile dark color="red" class="mt-4">
                Download Resume
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <div class="text-center mt-4">
        <h2>My projects</h2>
        <div style="width:120px; margin:0 auto">
          <v-slider v-model="slider2" color="red" :label="track-color"></v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="projects">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn icon="fas fa-laptop" color="#e81e5b" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Websites</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur
                </p>
              </div>
              <div class="child">
                <v-btn icon="fas fa-mobile-alt" color="#e81e5b" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Websites</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur
                </p>
              </div>
              <div class="child">
                <v-btn icon="fas fa-calculator" color="#e81e5b" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Websites</h3>
                <p class="text-grey ml-3 mt-4 text-caption">
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur<br/>
                  Lorem ipsum dolor sit amet consectetur
                </p>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" id="services">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#e81e5b" class="mr-2">All</v-btn>
          <v-btn class="mr-2" variant="tonal">Websites</v-btn>
          <v-btn class="mr-2" variant="tonal">git</v-btn>
          <v-btn class="mr-2" variant="tonal">Works</v-btn>
          <v-btn variant="tonal">Illustration</v-btn>
        </div>
      </v-col>
      <v-col cols="12" class="imgHover">
        <v-row class="fill-height" align="center" justify="center">
          <template v-for="(item,i) in items" :key="i">
            <v-col cols="12" md="4">
              <v-hover v-slot="{isHovering, props}">
                <v-card :elevation="isHovering ? 12: 2" :class="{'on-hover':isHovering}" v-bind="props">
                  <v-img :src="item.img" height="225px" cover></v-img>
                </v-card>
              </v-hover>
            </v-col>
          </template>
        </v-row>
      </v-col>
      <v-col cols="12" sm="12">
        <div class="d-flex justify-center mb-6">
          <v-btn color="#e81e5b" class="mt-4">Load more</v-btn>
        </div>
      </v-col>
      <v-col cols="12" id="page">
        <div class="pre">
          <v-row>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="i9.jpg" height="200px" cover></v-img>
                <v-card-title>We provide best</v-card-title>
                <v-card-subtitle>
                  By Selman | by git
                </v-card-subtitle>
                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat, obcaecati eum? Consequatur non pariatur hic.
                </v-card-text>
              </v-card>
            </v-col>
            <v-col cols="12" sm="4">
              <v-card class="mw-auto" max-width="344" height="">
                <v-img src="i9.jpg" height="200px" cover></v-img>
                <v-card-title>We provide best</v-card-title>
                <v-card-subtitle>
                  By Selman | by git
                </v-card-subtitle>
                <v-card-text>
                  Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat, obcaecati eum? Consequatur non pariatur hic.
                </v-card-text>
              </v-card>
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" id="blog">
        <div class="hire">
          <v-row>
            <v-col cols="12" sm="8">
              <h1 class="mt-9">Hire me</h1>
              <p class="text-grey">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Placeat, obcaecati eum? Consequatur non pariatur hic.
              </p>
            </v-col>
            <v-col cols="12" sm="4">
              <v-btn color="#e81e5b" class="mt-15">Hire me</v-btn>
            </v-col>
          </v-row>
        </div>
      </v-col>
    </v-container>
  </v-app>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '@/components/NavBar.vue';

export default defineComponent({
  name: 'HomeView',
  setup(){
    return {
      slider2:50,
      items:[
        {
          img:"i3.jpg",
        },
        {
          img:"i4.jpg",
        },
        {
          img:"i5.jpg",
        },
        {
          img:"i6.jpeg",
        },
        {
          img:"i8.jpg",
        },
        {
          img:"i9.jpg",
        },
      ],
    };
  },

  components: {
    NavBar,
  },
});
</script>
<style scoped>
.v-container{
  padding:16px 0;
}
.head{
  position: relative;
  text-align: center;
  padding: 12px;
  margin-bottom: 6px;
  height: 400px;
  width:100%;
  color: white;
}
.head:before{
  content: " ";
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width:50%;
  background: black;
  transform: skew(0deg,6deg);
}
.head::after{
  content: " ";
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width:50%;
  background: black;
  transform: skew(0deg,-6deg);
}
.egg{
  display: block;
  margin-left: 100px;
  margin-top: 50px;
  width: 356px;
  height: 300px;
  background-color: #f04141;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
.first{
  width: 100%;
  height: 280px;
  text-align:center;
  padding: 2rem 2rem;
}
.child{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover{
  padding: 0 200px;
}
.pre{
  width: 100%;
  height: 380px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}
.hire{
  width: 100%;
  height: 200px;
  padding:0 200px;
  background-color: #e9e9e9;
  margin-top: -24px; 
}
</style>
