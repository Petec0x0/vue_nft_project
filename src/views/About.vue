<template>
  <div class="home">
    <div class="mx-5 mx-auto">
      <div class="home-block d-flex">
        <section class="home-sidebar">
          <div class="home-sidebar__logo-box d-flex align-items-center">
            <div class="me-2"><img src="../assets/logo.png" alt="Logo"></div>
            <div class="home-sidebar__logo-text fw-bold">QuestNFT</div>
          </div>
          <ArmyComponent />
          <Collectibles />
          <Alliance />
        </section>
        <section class="home-main">
          <nav class="home-navbar">
          <Navbar />
          </nav>
          <main class="home-content">
            <ShowGeolocation />
            <Cards />
          </main>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import ArmyComponent from "@/components/armyComponent.vue"
import Collectibles from "@/components/Collectibles.vue"
import Cards from '@/components/cards.vue'
import Navbar from "../components/Navbar.vue"
import Alliance from "../components/Alliance.vue"
import ShowGeolocation from "../components/showGeolocation.vue"
export default {
  components: {
    ArmyComponent,
    Collectibles,
    Cards,
    Navbar,
    Alliance,
    ShowGeolocation
  }
}
</script>

<style scoped>
.home-block {
  background-color: aquamarine;
  height: 100vh;
}
.home-sidebar {
  background-color: rgba(34, 34, 34, 1);
  width: 25%;
  padding: 30px;
  overflow-y: scroll;
}
.home-sidebar__logo-box {
  margin-bottom: 40px;
}
.home-sidebar__logo-text {
  font-size: 24px;
  color: #fff;
  letter-spacing: 0.3rem;
}
.home-sidebar::-webkit-scrollbar{
  width: 7px;
}
.home-navbar {
}
.home-main {
  background-color: silver;
  width: 75%;
  position: relative;
}
.home-content {
  background-color: skyblue;
}
</style>