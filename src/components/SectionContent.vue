<script setup lang="ts"></script>

<template>
  <section>
    <div class="container">
      <!-- content -->
      <div class="content">
        <!-- img -->
        <div class="img">
          <img src="../assets/Section/image-product-1.jpg" alt="" />
        </div>
        <!-- description -->
        <div class="description">
          <!-- head title card  -->
          <div class="head-titles">
            <h3>Sneaker Company</h3>
            <!-- head title -->
            <h1>Fall Limited Edition Sneakers</h1>
            <!-- paragprh -->
            <p>
              These low-profile sneakers are your perfect casual wear companion.
              faturing a durable rubber outer sole , they'll withstand
              everything the weather can offer.
            </p>
          </div>

          <!-- pricing -->
          <div class="pricing">
            <div class="price">
              <span>$125.00</span>
              <a href="#">50%</a>
            </div>

            <!-- before pricing -->
            <div class="before_pricing">
              <p>$250.00</p>
            </div>
          </div>
          <div class="basket">
            <div class="counter">
              <span>-</span>
              <h3>0</h3>
              <span>+</span>
            </div>
            <div class="add">
              <img src="../assets/HeaderSvg/basket.svg" alt="" />
              <span>Add To Cart</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  min-height: 600px;
}
.content {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 600px;
  .img {
    width: 450px;
    height: 450px;
    img {
      width: 100%;
      height: 100%;
      border-radius: 5px;
    }
  }

  .description {
    display: flex;
    flex-direction: column;
    width: 350px;
    margin-left: 50px;
    .head-titles {
      h3 {
        color: rgb(255, 125, 26);
        text-align: left;
      }
      h1 {
        color: black;
        font-weight: bold;
        font-size: 30px;
        text-align: left;
      }
      p {
        text-align: justify;
        color: rgb(104, 112, 125);
      }
    }
    .pricing {
      display: flex;
      flex-direction: column;
      .price {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        span {
          margin-right: 5px;
          font-weight: bold;
          font-size: 20px;
        }
        a {
          width: 40px;
          height: 20px;
          border-radius: 4px;
          display: inline;
          background: rgb(255, 237, 224);
          color: rgb(255, 125, 26);
        }
      }
      .before_pricing {
        display: flex;
        justify-content: flex-start;
        p {
          text-decoration: line-through;
          color: rgb(195, 201, 229);
        }
      }
    }
    .basket {
      display: flex;
      justify-content: space-between;
      .counter {
        display: flex;
        width: 150px;
        background: rgb(247, 248, 253);
        align-items: center;
        justify-content: space-around;
        border-radius: 4px;
        height: 42px;
        span {
          margin-right: 5px;
          color: rgb(255, 125, 26);
          cursor: pointer;
        }
      }
      .add {
        display: flex;
        align-items: center;
        justify-content: center;
        cursor: pointer;
        height: 40px;
        border-radius: 4px;
        padding: 0px 20px;
        background: rgb(255, 125, 26);
        img {
          color: rgb(255, 237, 224);
          margin-right: 8px;
        }
        span {
          color: rgb(255, 237, 224);
          font-size: 14px;
        }
      }
    }
  }
}
@media only screen and (max-width: 800px) {
  .content {
    flex-direction: column;
    align-items: flex-start !important;
    justify-content: center !important;
    .head-titles {
      h3,
      h1,
      p {
        text-align: center;
      }
    }
  }
}
</style>
