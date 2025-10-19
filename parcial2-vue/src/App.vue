<template>
  <div>
    <header>
      <img src="./assets/roman.png" alt="Logo" class="logo" />
      <input type="text" placeholder="Buscar..." class="search-bar" />
      <nav>
        <button
          v-for="link in links"
          :key="link"
          @click="currentView = link"
          class="nav-link"
          :class="{ active: currentView === link }"
        >
          {{ link.charAt(0).toUpperCase() + link.slice(1) }}
        </button>
      </nav>
    </header>

    <main id="main-content">
      <component :is="componentsMap[currentView]" />
    </main>

    <footer>
      <p>© 2025 GERSSON VALENCIA - Web 1</p>
    </footer>
  </div>  
</template>

<script setup>
import { ref } from "vue";
import ChildrenMuro from "./components/children-muro.vue";
import ChildrenInfo from "./components/children-info.vue";
import ChildrenPhotos from "./components/children-photos.vue";
import ChildrenBoxes from "./components/children-boxes.vue";

const currentView = ref("muro");

const componentsMap = {
  muro: ChildrenMuro,
  info: ChildrenInfo,
  photos: ChildrenPhotos,
  boxes: ChildrenBoxes,
};

const links = ["muro", "info", "photos", "boxes"];
</script>


<style scoped>
:global(html),
:global(body) {
  height: 100%;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
  background-color: #f0f2f5;
}

div {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: #4267B2;
  color: white;
  padding: 10px 20px;
}

.logo {
  height: 40px;
}

.search-bar {
  flex: 1;
  margin: 0 20px;
  padding: 8px;
  border-radius: 4px;
  border: none;
}

nav {
  display: flex;
  gap: 10px;
}

.nav-link {
  background-color: white;
  color: #4267B2;
  border: none;
  padding: 8px 12px;
  border-radius: 4px;
  cursor: pointer;
}

main {
  flex: 1;
  padding: 20px;
}

footer {
  text-align: center;
  padding: 10px;
  background-color: #ddd;
}

</style>


