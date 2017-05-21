<template>
  <q-layout>
      <div slot="header" class="toolbar">
        <!-- opens drawer using its ref -->
        <button class="hide-on-drawer-visible" @click="$refs.leftDrawer.open()">
          <i>menu</i>
        </button>
        <q-toolbar-title :padding="2">
          Lean App Tools
        </q-toolbar-title>
        <button>
          <i>mail</i>
        </button>
        <button>
          <i>alarm</i>
        </button>
      </div>
      <q-drawer ref="leftDrawer">
        <div class="toolbar light">
          <q-toolbar-title :padding="1">
              TOOLS
          </q-toolbar-title>
        </div>
        <div class="list no-border platform-delimiter">
          <q-drawer-link icon="alarm" to="/takt">
            Takt Time
          </q-drawer-link>
          <q-drawer-link icon="alarm" to="/oee">
            OEE - Eficiency
          </q-drawer-link>
        </div>
      </q-drawer>
       <router-view class="layout-view"></router-view>
  </q-layout>
</template>
