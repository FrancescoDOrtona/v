<template>
  <footer class="page-footer">
    <div class="container">
      <div class="row footer-content">
        <div class="col page-footer__info">
          <h3>Boolando S.r.l.</h3>
          <ul class="footer-info">
            <li v-for="(info, index) in infos">{{ info }}</li>
          </ul>
        </div>
        <div class="col page-footer__social">
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
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
}

.container{
  max-width: 900px;
  margin: 0 auto;
}

.footer-content{
  justify-content: space-evenly;
  padding: 20px;
}

.footer-info{
  display: flex;
  gap: 15px;
  font-size: $font-size-sm;
}

.page-footer__info{
  display: flex;
  flex-direction: column;
  align-items: start;
}

.page-footer__social{
  display: flex;
  flex-direction: column;
  align-items: center;
}

h3{
  font-size: $font-size-md;
}
.page-footer__icons{
  display: flex;
  gap: 10px;
}
</style>