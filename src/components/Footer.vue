<template>
  <footer class="page-footer">
    <div class="container">
      <div class="row">
        <div class="col page-footer__info">
          <h3>Boolando S.r.l.</h3>
          <ul class="footer-info">
            <li v-for="(info, index) in infos">{{ info }}</li>
          </ul>
        </div>
        <div class="col">
          <h3>Trovaci anche su:</h3>
          <ul class="page-footer__icons">
            <li v-for="(social, index) in socials">
              <a href=""><font-awesome-icon :icon="social" /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
      data() {
        return {
            infos: ['Informazioni legali', 'Informativa sulla privacy', 'Diritto di recesso'],
            socials: ['fa-brands fa-twitter','fa-brands fa-facebook','fa-brands fa-instagram','fa-brands fa-pinterest','fa-brands fa-youtube' ]
        }
      }
    }
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.page-footer{
  background-color: $footer-color;
  width: 100%;
  display: flex;
  justify-content: space-between;
}

.footer-info{
  display: flex;
  gap: 15px;
}

.page-footer__info{
  display: flex;
  flex-direction: column;
  align-items: start;
}

.page-footer__icons{
  display: flex;
  gap: 10px;
}
</style>