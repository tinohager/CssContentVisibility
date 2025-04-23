<script setup lang="ts"></script>

<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="q-pa-none" role="menu">
        <q-toolbar-title shrink> Quasar App </q-toolbar-title>
        <q-item
          clickable
          exact
          active-class="text-white bg-grey-8 inset-shadow"
          role="menuitem"
          to="/"
        >
          <q-item-section class="text-uppercase text-weight-medium"> Home </q-item-section>
        </q-item>
        <q-item
          clickable
          exact
          active-class="text-white bg-grey-8 inset-shadow"
          role="menuitem"
          to="page1"
        >
          <q-item-section class="text-uppercase text-weight-medium"> Page1 </q-item-section>
        </q-item>
        <q-item
          clickable
          exact
          active-class="text-white bg-grey-8 inset-shadow"
          role="menuitem"
          to="page2"
        >
          <q-item-section class="text-uppercase text-weight-medium"> Page2 </q-item-section>
        </q-item>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>
