<template>
    <div class="card" v-for="(product,index) in products" :key="product.id">
        <img :src="product.frontImage" alt="">
        <div class="card-info">
            <h3>{{ product.brand }}</h3>
            <p>{{ product.name }}</p>
            <small>{{ product.price }}</small>
            <img src="" alt="">
        </div>
    </div>
</template>

<script>
    export default {
      data() {
        return {
            products: [
    {
      "id": 1,
      "frontImage": "/1.webp",
      "backImage": "1b.webp",
      "brand": "Levi's",
      "name": "Relaxed Fit",
      "price": 29.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 2,
      "frontImage": "/2.webp",
      "backImage": "2b.webp",
      "brand": "Guess",
      "name": "Roses Tee",
      "price": 20.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "discount",
          "value": "-30%"
        }
      ]
    },
    {
      "id": 3,
      "frontImage": "/3.webp",
      "backImage": "3b.webp",
      "brand": "Come Zucchero Filato",
      "name": "Voglia di colori pastello",
      "price": 129.99,
      "isInFavorites": false,
      "badges": [
        {
          "type": "discount",
          "value": "-30%"
        }
      ]
    },
    {
      "id": 4,
      "frontImage": "/4.webp",
      "backImage": "4b.webp",
      "brand": "Levi's",
      "name": "Tee Unisex",
      "price": 14.99,
      "isInFavorites": false,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 5,
      "frontImage": "/5.webp",
      "backImage": "5b.webp",
      "brand": "Maya Deluxe",
      "name": "Stripe Bodice",
      "price": 99.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        },
        {
          "type": "discount",
          "value": "-50%"
        }
      ]
    },
    {
      "id": 6,
      "frontImage": "/6.webp",
      "backImage": "6b.webp",
      "brand": "Esprit",
      "name": "Maglione - Black",
      "price": 29.99,
      "isInFavorites": true,
      "badges": [
        {
          "type": "tag",
          "value": "Sostenibilità"
        }
      ]
    }
  ]
        }
      }
    }

</script>

<style lang="scss" scoped>
.card-info{
    display: flex;
    flex-direction: column;
    gap: 5px;
}
</style>