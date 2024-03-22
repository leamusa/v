<script>
export default {
  name: "Main",
  data() {
    return {
      card: [
        {
          id: 1,
          frontImage: "1.webp",
          backImage: "1b.webp",
          brand: "Levi's",
          name: "Relaxed Fit",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 2,
          frontImage: "2.webp",
          backImage: "2b.webp",
          brand: "Guess",
          name: "Roses Tee",
          price: 20.99,
          isInFavorites: true,
          badges: [
            {
              type: "discount",
              value: "-30%",
            },
          ],
        },
        {
          id: 3,
          frontImage: "3.webp",
          backImage: "3b.webp",
          brand: "Come Zucchero Filato",
          name: "Voglia di colori pastello",
          price: 129.99,
          isInFavorites: false,
          badges: [
            {
              type: "discount",
              value: "-30%",
            },
          ],
        },
        {
          id: 4,
          frontImage: "4.webp",
          backImage: "4b.webp",
          brand: "Levi's",
          name: "Tee Unisex",
          price: 14.99,
          isInFavorites: false,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 5,
          frontImage: "5.webp",
          backImage: "5b.webp",
          brand: "Maya Deluxe",
          name: "Stripe Bodice",
          price: 99.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
            {
              type: "discount",
              value: "-50%",
            },
          ],
        },
        {
          id: 6,
          frontImage: "6.webp",
          backImage: "6b.webp",
          brand: "Esprit",
          name: "Maglione - Black",
          price: 29.99,
          isInFavorites: true,
          badges: [
            {
              type: "tag",
              value: "Sostenibilità",
            },
          ],
        },
      ],
    };
  },
  methods: {
    getImagePath(img) {
      return require(`@/public/img/${img}`);
    },
  },
};
</script>
<template>
  <div>
    <div class="main-container">
      <div class="img-card">
        <a href="#">
          <img src="/img/2.webp" alt="" class="img-main" />
          <img src="/img/2b.webp" alt="" class="img-hover" />
        </a>
        <span class="discount">-30%</span>
        <span class="heart"> &hearts;</span>
      </div>
      <div class="product-description">
        <p>Guess</p>
        <h3>ROSES TEE</h3>
        <p>
          <span class="price">20,99 &euro;</span>
          <span class="ex-price">29,99 &euro;</span>
        </p>
      </div>
    </div>

    <div class="main-container">
      <div class="img-card">
        <a href="#">
          <img src="/img/3.webp" alt="" class="img-main" />
          <img src="/img/3.webp" alt="" class="img-hover" />
        </a>
        <span class="discount">-30%</span>
        <span class="heart"> &hearts;</span>
      </div>
      <div class="product-description">
        <p>Come Zucchero Filato</p>
        <h3>VOGLIA DI COLORI PASTELLO</h3>
        <p>
          <span class="price">129,99 &euro;</span>
          <span class="ex-price">184,99 &euro;</span>
        </p>
      </div>
    </div>

    <div class="main-container">
      <div class="img-card">
        <a href="#">
          <img src="/img/4.webp" alt="" class="img-main" />
          <img src="/img/4b.webp" alt="" class="img-hover" />
        </a>
        <span class="discount">-50%</span>
        <span class="ecological">Sostenibilità</span>
        <span class="heart"> &hearts;</span>
      </div>
      <div class="product-description">
        <p>Levi's</p>
        <h3>TEE UNISEX</h3>
        <p>
          <span class="price">14,99 &euro;</span>
          <span class="ex-price">29.99 &euro;</span>
        </p>
      </div>
    </div>

    <div class="main-container">
      <div class="img-card">
        <a href="#">
          <img src="/img/5.webp" alt="" class="img-main" />
          <img src="/img/5b.webp" alt="" class="img-hover" />
        </a>
        <span class="heart"> &hearts;</span>
      </div>
      <div class="product-description">
        <p>Maya Deluxe</p>
        <h3>STRIPE BODICE</h3>
        <p><span class="price">14,99 &euro;</span></p>
      </div>
    </div>

    <div class="main-container">
      <div class="img-card">
        <a href="#">
          <img src="/img/6.webp" alt="" class="img-main" />
          <img src="/img/6b.webp" alt="" class="img-hover" />
        </a>
        <span class="ecological-no-discount">Sostenibilità</span>
        <span class="heart"> &hearts;</span>
      </div>
      <div class="product-description">
        <p>Esprit</p>
        <h3>MAGLIONE - BLACK</h3>
        <p><span class="price">29,99 &euro;</span></p>
      </div>
    </div>
  </div>
</template>

<style></style>
