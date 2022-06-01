<template>
    <body>
    <sidebar />
    <section class="home-section">
        <navbar />
        <div class="home-content">
        </div>
        <div class="container-fluid">
            <div class="row">
                <div class="copyright">
                    <p>Copyright © 2022 <strong> Vortens LTDA</strong>. Todos os direitos reservados.</p>
                </div>
            </div>
        </div>
        </section>
    </body>
</template>

<script>
import Navbar from '../components/Navbar.vue'
import Sidebar from '../components/Sidebar.vue'

export default {
  components: {
    Sidebar,
    Navbar
  },
  name: 'Dashboard'
}
</script>

<style>
/* @import '../styles/styles.css'; */

</style>
