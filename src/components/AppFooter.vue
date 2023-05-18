<script></script>

<template>
  <footer>
    <div class="top-footer-bg">
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
    <div class="middle-footer-bg">
      <div class="container">
        <div class="middle-footer">
          <div class="lists">
            <ul class="comics">
              <li><h2>dc comics</h2></li>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>

            <ul class="shop">
              <li><h2>shop</h2></li>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>

            <ul class="dc">
              <li><h2>dc</h2></li>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contacs Us</li>
            </ul>

            <ul class="sites">
              <li><h2>sites</h2></li>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
          <img src="./../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="bottom-footer-bg">
      <div class="container">
        <div class="bottom-footer">
          <button class="sign-up">sign-up now!</button>
          <ul class="socials">
            <li><h2>follow us</h2></li>
            <li><img src="./../assets/img/footer-facebook.png" alt="" /></li>
            <li><img src="./../assets/img/footer-twitter.png" alt="" /></li>
            <li><img src="./../assets/img/footer-youtube.png" alt="" /></li>
            <li><img src="./../assets/img/footer-pinterest.png" alt="" /></li>
            <li><img src="./../assets/img/footer-periscope.png" alt="" /></li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.top-footer-bg {
  background-color: #0282f9;
}

.middle-footer-bg {
  background-image: url("./../assets/img/footer-bg.jpg");
}

.bottom-footer-bg {
  background-color: #303030;
}

.container {
  width: 960px;
  max-width: 1280px;
  margin: 0 auto;
}

.top-footer {
  height: 120px;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  color: white;
}

.top-footer {
  section {
    padding: 0.5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0.3rem;
  }

  section {
    img {
      display: block;
      height: 40px;
      aspect-ratio: 1 / 1;
      object-fit: contain;
    }

    h2 {
      font-weight: 400;
      font-size: 0.7rem;
      text-transform: uppercase;
    }
  }
}

.middle-footer {
  height: 350px;
  display: grid;
  grid-template-columns: repeat(9, 1fr);
  color: rgba(255, 255, 255, 0.4);
  overflow: hidden;
}

.middle-footer {
  .lists {
    padding: 2rem 0;
    grid-column: 1 / 4;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(7, 35px);
    column-gap: 0.5rem;
  }

  .lists {
    h2 {
      color: white;
      text-transform: uppercase;
      font-size: 1rem;
      margin-bottom: 0.7rem;
    }

    li {
      line-height: 1.1rem;
      font-size: 0.6rem;
    }

    .comics {
      grid-column: 1 / 2;
      grid-row: 1 / 6;
    }

    .shop {
      grid-column: 1 / 2;
      grid-row: 6 / 8;
    }

    .dc {
      grid-column: 2 / 3;
    }

    .sites {
      grid-column: 3 / 4;
    }
  }

  img {
    grid-column: 6 / 10;
    display: block;
    height: 121%;
    align-self: center;
  }
}

.bottom-footer {
  height: 82px;
  display: grid;
  align-items: center;
  grid-template-columns: repeat(9, 1fr);
}

.bottom-footer {
  .sign-up {
    grid-column: 1 / 2;
    padding: 0.6rem;
    font-size: 0.7rem;
    font-weight: 600;
    text-transform: uppercase;
    color: white;
    background-color: unset;
    border: unset;
    border: 1px solid #0c7af3;
  }

  .socials {
    grid-column: 7 / 10;
    display: flex;
    gap: 1rem;
    align-items: center;
  }

  h2 {
    font-size: 1rem;
    text-transform: uppercase;
    color: #0c7af3;
  }

  li > img {
    display: block;
    width: 25px;
    aspect-ratio: 1 / 1;
  }
}
</style>
