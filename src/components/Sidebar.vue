<template>
  <div class="sidebar">
    <div class="logo-details">
      <img src="../assets/logoWhite.svg" width="650px" height="250px">
      <!-- <span class="logo_name">VortensAdmin</span> -->
    </div>
    <ul class="nav-links" style="padding-left: 0rem;">
        <li>
          <a href="#" class="active">
            <i><font-awesome-icon icon="fa-solid fa-square-poll-horizontal" /></i>
            <span class="links_name">Dashboard</span>
          </a>
        </li>
        <li>
          <a href="#">
            <i><font-awesome-icon icon="fa-solid fa-address-book" /></i>
            <span class="links_name">Clientes</span>
          </a>
        </li>
        <li>
          <a href="#">
            <i><font-awesome-icon icon="fa-solid fa-tag" /></i>
            <span class="links_name">Planos</span>
          </a>
        </li>
        <li>
          <a href="#">
            <i><font-awesome-icon icon="fa-solid fa-cart-shopping" /></i>
            <span class="links_name">Pedidos</span>
          </a>
        </li>
        <li>
          <a href="#">
            <i><font-awesome-icon icon="fa-solid fa-users" /></i>
            <span class="links_name">Parceiros Comerciais</span>
          </a>
        </li>
        <li>
          <a href="#">
            <i><font-awesome-icon icon="fa-solid fa-address-card" /></i>
            <span class="links_name">Leads</span>
          </a>
        </li>
        <li class="log_out">
          <a href="#">
            <i><font-awesome-icon icon="fa fa-sign-out-alt" /></i>
            <span class="links_name">Log out</span>
          </a>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: 'Sidebar'
}
</script>

<style>
/* @import '../styles/styles.css'; */

</style>
