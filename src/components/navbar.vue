<template>
    <q-header elevated>
      <q-toolbar>
        <q-btn flat round dense icon="menu" @click="$refs.leftDrawer.open()" />
        <q-toolbar-title>
          <span>Skincare Shop</span>
        </q-toolbar-title>
        <q-space />
        <q-input class="input" placeholder="Cari Produk Skin Care"></q-input>
        <q-btn flat round dense icon="search" />
        <q-btn flat round dense icon="shopping_cart" />
        <q-menu>
          <q-btn flat dense label="Menu" icon="menu" slot="trigger"></q-btn>
          <q-list>
            <q-item clickable v-close-popup>
              <q-item-section>
                <q-item-label>Facial Wash</q-item-label>
              </q-item-section>
            </q-item>
            <q-item clickable v-close-popup>
              <q-item-section>
                <q-item-label>Foundation</q-item-label>
              </q-item-section>
            </q-item>
            <q-item clickable v-close-popup>
              <q-item-section>
                <q-item-label>Serum</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
        </q-menu>
        <q-btn flat dense label="Home" />
        <q-btn flat dense label="Tentang Kami" />
        <q-btn flat dense label="Hubungi Kami" />
      </q-toolbar>
    </q-header>
  </template>
  
  <script>
  export default {};
  </script>
  
  <style scoped>
  .q-header {
    background-color: #c78f00;
    color: #FFF;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .q-btn {
    color: #FFF;
  }
  
  .q-btn:hover {
    background-color: rgba(255, 255, 255, 0.1);
  }

  .input {
    background-color: #b78300;
    border-radius: 20px;
    padding: 0px 30px;
  }
  </style>
  