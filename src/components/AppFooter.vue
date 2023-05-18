<script></script>

<template>
  <footer>
    <div class="container-bg">
      <div class="container">
        <div class="top-footer">
          <section>
            <img src="./../assets/img/buy-comics-digital-comics.png" alt="" />
            <h2>digital comics</h2>
          </section>
          <section>
            <img src="./../assets/img/buy-comics-merchandise.png" alt="" />
            <h2>dc merchandise</h2>
          </section>
          <section>
            <img src="./../assets/img/buy-comics-subscriptions.png" alt="" />
            <h2>subscription</h2>
          </section>
          <section>
            <img src="./../assets/img/buy-comics-shop-locator.png" alt="" />
            <h2>comic shop locator</h2>
          </section>
          <section>
            <img src="./../assets/img/buy-dc-power-visa.svg" alt="" />
            <h2>dc power visa</h2>
          </section>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.container-bg {
  background-color: #0282f9;
}

.container {
  width: 960px;
  max-width: 1280px;
  margin: 0 auto;
}

.top-footer {
  height: 150px;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  color: white;
}

.top-footer {
  section {
    padding: 0.6rem;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0rem;
  }
  section {
    img {
      display: block;
      height: 38px;
      width: 38px;
      object-fit: contain;
    }

    h2 {
      font-weight: 400;
      font-size: 0.7rem;
      text-transform: uppercase;
    }
  }
}
</style>
