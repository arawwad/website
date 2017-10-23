<template>
  <b-container  id="skills">
    <b-row class="text-center">
      <b-col>
        <h2>Skills</h2>
        <starlight></starlight>
      </b-col>
    </b-row>
    <b-row class="text-center mt-5" >
      <b-col cols="12" sm="4" v-for="skill in skills" :key="skill.name" class="my-3 skill">
        <span v-b-toggle="skill.name" :class="skill.class" :id="skill.name" class="dev-icon"></span>
        <p>{{skill.name}}</p>
        <b-collapse :id="skill.name" class="mt-2">
          <b-card>{{skill.note}}</b-card>
        </b-collapse>
      </b-col>
    </b-row>
  </b-container>
</template>


<script>
  import Starlight from './Starlight.vue'
  export default {
    name: 'Skills',
    data () {
      return {
        skills: [
          {
            name: 'HTML 5',
            class: 'devicon-html5-plain',
            note: 'HTML5 is the latest evolution of the standard that defines HTML. The term represents two different concepts. It is a new version of the language HTML, with new elements, attributes, and behaviors, and a larger set of technologies that allows the building of more diverse and powerful Web sites and applications'
          },
          {
            name: 'CSS 3',
            class: 'devicon-css3-plain',
            note: 'CSS3 is the latest evolution of the Cascading Style Sheets language and aims at extending CSS2.1. It brings a lot of long-awaited novelties, like rounded corners, shadows, gradients, transitions or animations, as well as new layouts like multi-columns, flexible box or grid layouts.'
          },
          {
            name: 'JAVASCRIPT',
            class: 'devicon-javascript-plain',
            note: 'JavaScript is a high-level, dynamic, weakly typed, prototype-based, multi-paradigm, and interpreted programming language. Alongside HTML and CSS, JavaScript is one of the three core technologies of World Wide Web content production. It is used to make webpages interactive and provide online programs, including video games.'
          },
          {
            name: 'BOOTSTRAP',
            class: 'devicon-bootstrap-plain',
            note: 'Bootstrap was made to not only look and behave great in the latest desktop browsers, but in tablet and smartphone browsers via responsive CSS. A 12-column responsive grid, dozens of components, JavaScript plugins, typography, form controls, and even a web-based Customizer to make Bootstrap your own.'
          },
          {
            name: 'VUE.JS',
            class: 'devicon-vuejs-plain',
            note: 'Vue.js is an open-source progressive JavaScript framework for building user interfaces. Integration into projects that use other JavaScript libraries is made easy with Vue because it is designed to be incrementally adoptable.'
          },
          {
            name: 'JQUERY',
            class: 'devicon-jquery-plain',
            note: 'jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers.'
          },
          {
            name: 'SASS',
            class: 'devicon-sass-plain',
            note: 'Sass is the most mature, stable, and powerful professional grade CSS extension language in the world.'
          },
          {
            name: 'NODE.JS',
            class: 'devicon-nodejs-plain',
            note: 'Node.js is a JavaScript runtime built on Chrome\'s V8 JavaScript engine. Node.js uses an event-driven, non-blocking I/O model that makes it lightweight and efficient. Node.js\' package ecosystem, npm, is the largest ecosystem of open source libraries in the world.'
          },
          {
            name: 'EXPRESS',
            class: 'devicon-express-original',
            note: 'Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.'
          },
          {
            name: 'GIT',
            class: 'devicon-git-plain',
            note: 'Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency. Git is easy to learn and has a tiny footprint with lightning fast performance'
          },
          {
            name: 'GITHUB',
            class: 'devicon-github-plain',
            note: 'GitHub is a web-based Git or version control repository and Internet hosting service. It is mostly used for code. It offers all of the distributed version control and source code management functionality of Git as well as adding its own features.'
          },
          {
            name: 'CHROME DEV TOOLS',
            class: 'devicon-chrome-plain',
            note: 'The Chrome Developer Tools, are a set of web authoring and debugging tools built into Google Chrome. The DevTools provide web developers deep access into the internals of the browser and their web application. Use the DevTools to efficiently track down layout issues, set JavaScript breakpoints, and get insights for code optimization.'
          },
          {
            name: 'WEBPACK',
            class: 'devicon-webpack-plain',
            note: 'webpack is a module bundler for modern JavaScript applications. When webpack processes your application, it recursively builds a dependency graph that includes every module your application needs, then packages all of those modules into a small number of bundles - often only one - to be loaded by the browser.'
          },
          {
            name: 'BABEL',
            class: 'devicon-babel-plain',
            note: 'The compiler for writing next generation JavaScript.'
          },
          {
            name: 'WEBSTORM',
            class: 'devicon-webstorm-plain',
            note: 'Use the full power of the modern JavaScript ecosystem with the intelligent code completion, on-the-fly error detection, powerful navigation and refactoring for JavaScript, TypeScript, stylesheet languages, and the most popular frameworks.'
          },
          {
            name: 'VS CODE',
            class: 'devicon-visualstudio-plain',
            note: 'Visual Studio Code is a lightweight but powerful source code editor. It comes with built-in support for JavaScript, TypeScript and Node.js'
          }
        ]
      }
    },
    components: {
      Starlight
    }
  }
</script>

<style lang="scss" scoped>
.container{
  padding:60px 0;
}

.col h2{
  font-weight:bold;
  font-family: 'Montserrat', sans-serif;
  color: #000;
  font-size: 4rem;
}
.col p{
  font-family: 'lato', sans-serif;
}
hr.star-light::after {
  background-color: white;
}
  .dev-icon{
    font-size: 4rem;
    color: #17a2b8;
  }

  span:hover{
    border-color:black;
    cursor: pointer;
  }

span:hover {
  content: "\e7f7";
  border: 5px solid #f1f1f1;
  padding: 25px;
  background-color: #18BC9C;
}

</style>
