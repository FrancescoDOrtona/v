<template>
    <div class="page-store">
        <div class="container">
            <div class="grid">
                <Card/>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue'

export default {
    components:{
        Card,
    },
      data() {
        return {
        }
      }
    }

</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.page-store{
    margin-top: 100px;
    color: black;
    text-align: center;
}

.container {
    max-width: 1024px;
    margin: 0 auto;
  }

  .grid{
    display: grid;
    grid-template-columns: repeat(3,1fr);
  }
</style>