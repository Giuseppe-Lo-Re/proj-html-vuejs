<template>
    <main>

      <!-- "Start Investing" Section -->
      <StartInvesting />
      
      <!-- "Course List" Section -->
      <CourseList />

      <!-- "Limitess Learning" Section -->
      <LimitessLearning />

      <!-- "Recent Course" Section -->
      <RecentCourse />

      <!-- "We are Proud" Section -->
      <WeareProud />

      <!-- Newsletter Section -->
      <NewsLetter />

      <!-- "Popular Course" Section -->
      <PopularCourse />

      <!-- "Instructor/Business" Section -->
      <InstructorBusiness />

      <!-- "Come As You Are" Section -->
      <ComeasYouare />
    </main>
</template>

<script>
import StartInvesting from "../components/StartInvesting";
import CourseList from "../components/CourseList";
import LimitessLearning from "../components/LimitessLearning";
import RecentCourse from "../components/RecentCourse";
import WeareProud from "../components/WeareProud";
import NewsLetter from "../components/NewsLetter";
import PopularCourse from "../components/PopularCourse";
import InstructorBusiness from "../components/InstructorBusiness";
import ComeasYouare from "../components/ComeasYouare";

export default {
  name: "MainComponent",
  components: {
    StartInvesting,
    CourseList,
    LimitessLearning,
    RecentCourse,
    WeareProud,
    NewsLetter,
    PopularCourse,
    InstructorBusiness,
    ComeasYouare
  }
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";
</style>