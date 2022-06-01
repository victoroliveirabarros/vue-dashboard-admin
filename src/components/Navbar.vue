<template>
    <nav>
      <div class='sidebar-button'>
        <i class='bx bx-menu sidebarBtn' @click='resizeBar'></i>
        <span class='dashboard medium-font'>Vortens Tecnologia</span>
      </div>
      <div class='profile-details' @click='collapse_settings_header_top'>
        <!--<img src='images/profile.jpg' alt=''>-->
        <span class='admin_name'>Victor Oliveira Barros do Nascimento</span>
        <i><font-awesome-icon icon="fa-solid fa-circle-user" /></i>
        <i class='bx bx-chevron-down' ></i>
      </div>
      <div class='setting-menu'>
        <ul class="nav-links" style="padding-left: 0rem;">
          <li>
            <a href="#">
                <i><font-awesome-icon icon="fa-solid fa-gear" /></i>
                <span class="links_name">Gerenciar</span>
            </a>
          </li>
          <li>
              <a href="#">
                  <i><font-awesome-icon icon="fa-solid fa-fingerprint" /></i>
                  <span class="links_name">Alterar senha</span>
              </a>
          </li>
        </ul>
      </div>
    </nav>
</template>

<script>
export default {
  name: 'Navbar',
  methods: {
    resizeBar () {
      let sidebar = document.querySelector('.sidebar')
      let sidebarBtn = document.querySelector('.sidebarBtn')

      sidebarBtn.onclick = function () {
        sidebar.classList.toggle('active')
        if (sidebar.classList.contains('active')) {
          sidebarBtn.classList.replace('bx-menu', 'bx-menu-alt-right')
        } else {
          sidebarBtn.classList.replace('bx-menu-alt-right', 'bx-menu')
        }
      }
    },
    collapse_settings_header_top () {
      this.toggle('.setting-menu', 'show-setting-menu')
      // document.querySelector('.setting-menu').style.display = 'block'
      // document.querySelector('.setting-menu').style.right = '4px'
    },
    toggle (el, classname) {
      var element = document.querySelector(el)
      console.log(element.classList)
      if (element.classList.contains(classname)) {
        element.classList.remove(classname)
        document.querySelector('.setting-menu').style.display = 'none'
        document.querySelector('.setting-menu').style.right = '-300px'
      } else {
        element.classList.add(classname)
        document.querySelector('.setting-menu').style.display = 'block'
        document.querySelector('.setting-menu').style.right = '4px'
      }
    }
  }
}
</script>

<style>

</style>
