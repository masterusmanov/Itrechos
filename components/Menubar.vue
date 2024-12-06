<template>
     <div class="">
      <button class="fixed-menu" @click="toggleMenu">
        &#9776;
      </button>
        <nav v-if="isOpen" class="menu">
          <ul>
            <li>
              <a href="#home">Home</a>
            </li>
            <li>
              <a href="#service">Services</a>
            </li>
            <li>
              <a href="#page">Pages</a>
            </li>
            <li>
              <a href="#blog">Blog</a>
            </li>
            <li>
              <a href="#contact">Contact</a>
            </li>
          </ul>
        </nav>
    </div>
</template>

<script setup>
    const isOpen = ref(false);

    const toggleMenu = () => {
    isOpen.value = !isOpen.value;
    };

</script>

<style lang="scss" scoped>
.fixed-menu {
    margin-top: 5px;
    position: fixed;
    top: 100px;
    right: 10px;
    font-size: 24px;
    z-index: 1000;
    color: white;
    padding: 10px;
    cursor: pointer;
}

.menu {
    background-color: #070706;
    position: fixed;
    top: 100px;
    right: 10px;
    width: 120px;
    border-radius: 5px;
    padding: 10px;
    z-index: 1000;
}

.menu ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

.menu ul li {
    margin: 10px 0;
}

.menu ul li a {
    color: white;
    text-decoration: none;
}

.fixed-menu {
    position: fixed;
    top: 15px;
    right: 10px;
    z-index: 1000;
    background-color: #070706;
    color: white;
    padding: 8px 10px;
    border-radius: 5px;
    cursor: pointer;
}
</style>