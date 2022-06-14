<script setup lang="ts">
import { ref } from "vue";

const open = ref(true)

</script>

<template>
  <div class="sidebar">
    <div class="logo-details">
        <i class="fa-brands fa-codepen"></i>
      <span class="logo_name">CodingLab</span>
    </div>
    <ul class="nav-links">
      <li>
        <a href="#">
          <i class="fas fa-home"></i>
          <span class="link_name">Dashboard</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">Dashboard</a></li>
        </ul>
      </li>
      <li>
        <a href="#">
          <i class="fas fa-briefcase"></i>
          <span class="link_name">BID Opening</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">BID Opening</a></li>
        </ul>
      </li>
      <li @click="open = !open" :class="open ? 'showMenu' : '' ">
        <div class="icon-link">
          <a href="#">
            <i class="fas fa-coins"></i>
            <span class="link_name">Quote Opening</span>
          </a>
          <i class="fas fa-angle-down arrow"></i>
        </div>
        <ul class="sub-menu">
          <li><a class="link_name" href="#">Quote Opening</a></li>
          <li><a href="#">Quotation</a></li>
          <li><a href="#">Special Quote</a></li>
        </ul>
      </li>
      <li>
        <a href="#">
          <i class="fas fa-euro-sign"></i>
          <span class="link_name">Quotes</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">Quotes</a></li>
        </ul>
      </li>
      <li>
        <a href="#">
          <i class="fas fa-tag"></i>
          <span class="link_name">Categories</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">Categories</a></li>
        </ul>
      </li>
      <li @click="open = !open" :class="open ? 'showMenu' : ''">
        <div class="icon-link">
          <a href="#">
            <i class="fas fa-book"></i>
            <span class="link_name">Reports</span>
          </a>
          <i class="fas fa-angle-down arrow"></i>
        </div>
        <ul class="sub-menu">
          <li><a class="link_name" href="#">Reports</a></li>
          <li><a href="#">Per Period</a></li>
          <li><a href="#">Per Categories</a></li>
          <li><a href="#">Per Company</a></li>
          <li><a href="#">Per Provider</a></li>
        </ul>
      </li>
      <li>
        <a href="#">
          <i class="fas fa-user-tie"></i>
          <span class="link_name">Process</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">Process</a></li>
        </ul>
      </li>
      <li>
        <a href="#">
          <i class="fas fa-file-alt"></i>
          <span class="link_name">Documentation</span>
        </a>
        <ul class="sub-menu blank">
          <li><a class="link_name" href="#">Documentation</a></li>
        </ul>
      </li>
      <li>
        <div class="profile-details">
          <div class="profile-content">
            <img src="./assets/images/avatar.png" alt="profile">
          </div>
          
          <div class="name-job">
            <div class="profile_name">
              <div class="profile_name">Vinícius Dias</div>
              <div class="job">Web Developer</div>
            </div>
          </div>
          <i class="fas fa-sign-out-alt"></i>
        </div>
      </li>
    </ul>
  </div>
  <section class="home-section">
    <div class="home-content">
      <i class="fas fa-bars"></i>
      <span class="text">Drop Down Sidebar</span>
    </div>
  </section>
</template>

<style>
@import "assets/styles.css";
</style>
