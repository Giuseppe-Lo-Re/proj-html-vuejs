<template>
  <div id="app">

    <!-- Header -->
    <HeaderComponent 
      :links="headerLinks"
      />

    <!-- Main -->
    <MainComponent />

    <!-- Footer -->
    <FooterComponent 
      :links1="footerLinks1"
      :links2="footerLinks2"/>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent";
import  MainComponent  from "./components/MainComponent";
import  FooterComponent  from "./components/FooterComponent";

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  },
  data() {
    return {
      headerLinks: [
         {
          category: 'Courses',
          url: '#',
          isNew: false
        },
        {
          category: 'Zoom',
          url: '#',
          isNew: true
        },
        {
          category: 'Pages',
          url: '#',
          isNew: false
        },
        {
          category: 'Bundles',
          url: '#',
          isNew: false
        },
        {
          category: 'Course Formats',
          url: '#',
          isNew: false
        },
        {
          category: 'Add Course',
          url: '#',
          isNew: true
        },
        {
          category: 'Demos',
          url: '#',
          isNew: false
        }
      ],
      footerLinks1: [
        {
          category: 'Blog',
          url: '#'
        },
        {
          category: 'Home',
          url: '#'
        },
        {
          category: 'Shortcodes',
          url: '#'
        }
      ],
      footerLinks2: [
        {
          category: 'Courses',
          url: '#'
        },
        {
          category: 'Membership',
          url: '#'
        },
        {
          category: 'Typography',
          url: '#'
        },
      ]
    } 
  }
}
</script>

<style lang="scss">
@import "./style/common.scss";

</style>
