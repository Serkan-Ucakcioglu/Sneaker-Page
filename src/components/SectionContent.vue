<script setup lang="ts"></script>

<template>
  <section>
    <div class="container">
      <div class="content">
        <div class="img">
          <img src="../assets/Section/image-product-1.jpg" alt="" />
        </div>
        <div class="description">
          <h3>Sneaker Company</h3>
          <h1>Fall Limited Edition Sneakers</h1>
          <p>These low-profile sneakers are your perfect casual wear companion. faturing a durable rubber outer sole , they'll withstand everything the weather can offer. </p>
          <div class="pricing">
            <span>$125.00</span>
            <a href="#">50%</a>
            <div class="before_pricing">
                <p>$250.00</p>
            </div>
          </div>
          <div class="basket"></div>
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

  height: 600px;
  .img {
    img {
      width: 450px;
      height: 450px;
      border-radius: 5px;
    }
  }

  .description {
    display: flex;
    flex-direction: column;
    width: 350px;
    margin-left:  50px;
    h3 {
      color: rgb(255, 125, 26);
    }
    h1{
        color: black;
        font-weight: bold;
        font-size: 35px;
    }
    p{
        text-align: justify;
        color: rgb(104, 112, 125);
    }
    .pricing{
        display: flex;
        span{
        margin-right: 5px;
        font-weight: bold;
        font-size: 20px;
        }
        a{
            width: 40px;
            height: 20px;
            border-radius: 4px;
            display: inline;
            background:rgb(255, 237, 224);
            color: rgb(255, 125, 26);
        }
    }
  }
}
</style>
