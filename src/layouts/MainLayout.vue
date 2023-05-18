<template>
  <q-layout view="hHh Lpr lFf">
    <q-header class="bg-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-img src="~assets/kd-logo.png" width="80px"></q-img>
        </q-toolbar-title>
<q-space />
        <q-input
          class="GNL__toolbar-input"
          outlined
          dense
          v-model="search"
          color="bg-grey-7 shadow-1 gt-xs"
          placeholder="Search"
        >
          <template v-slot:prepend>
            <q-icon v-if="search === ''" name="search" />
            <q-icon
              v-else
              name="clear"
              class="cursor-pointer"
              @click="search = ''"
            />
          </template>
        </q-input>
        <q-space />

        <div class="gt-sm text-black q-mx-sm">
          <q-btn round color="primary" icon="shopping_cart" class=" q-mx-sm" title="Add To Cart"/>
          <q-btn round color="primary" icon="fas fa-truck-fast" class=" q-mx-sm" title="Place Order"/>
          <q-btn round color="primary" icon="person" class=" q-mx-sm" title="My Account"/>
        </div>


        <div class="lt-md">
          <q-btn
            flat
            dense
            round
            icon="menu"
            aria-label="Menu"
            color="primary"
            @click="toggleLeftDrawer"
          />
        </div>
      </q-toolbar>
    </q-header>
    <q-drawer v-model="leftDrawerOpen" bordered dark>
      <q-list>
        <!-- <q-item-label header> Essential Links </q-item-label> -->

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
          class="text-center"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

     <footer class="bg-primary text-grey-8 q-mt-md">
      <q-toolbar>
        <q-space class="" />
        &copy; 2023 - All Rights Reserved - Kingdom Dynasty Limited
        <q-space />
      </q-toolbar>
    </footer>
  </q-layout>


</template>

<style scoped>
.GNL__toolbar-input {
  width: 50%;
}
</style>

<script>
import { defineComponent, ref } from "vue";
import EssentialLink from "components/EssentialLink.vue";

const linksList = [
  {
    title: "About",
    link: "#",
  },
  {
    title: "Service",
    link: "#",
  },
  {
    title: "Appointment",

    link: "#",
  },
  {
    title: "Gallery",
    link: "#",
  },
  {
    title: "Contact",
    link: "#",
  },
];

export default defineComponent({
  name: "MainLayout",

  components: {
    EssentialLink,
  },

  setup() {
    const leftDrawerOpen = ref(false);
    const search = ref("")

    return {
      search,
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      },
    };
  },
});
</script>
