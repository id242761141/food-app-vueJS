<template>
  <div class="home">
    <div class="header">
      <h2 class="title">Hi <b>Assylbek!</b></h2>
      <div class="input">
        <input type="text" placeholder="Find what you want..." />
        <div class="icon-input">
          <i class="bx bx-search"></i>
        </div>
      </div>
      <div class="combo-header">
        <div class="text">
          <h3>Free combo</h3>
          <p>Burger + Coca-cola for new users</p>
        </div>
        <div class="img">
          <img
            src="https://wkau.kz/wp-content/uploads/2022/02/png-clipart-whopper-hamburger-big-king-take-out-chicken-sandwich-burger-king-food-recipe.png"
            alt=""
          />
        </div>
      </div>
    </div>
    <div class="scroll-menu">
      <div class="scroll-content">
        <div :key="index" class="avatar" v-for="(item, index) in 40">
          <i class="bx bxs-pizza bx-sm"></i>
          <div class="title">
            Pizza
          </div>
        </div>
      </div>
    </div>
    <h2>Top Products</h2>
    <div class="top-products-all">
      <div :key="index" class="top-products" v-for="(items, index) in 40">
        <div class="top-products-img">
          <img
            src="https://www.pngplay.com/wp-content/uploads/6/Berry-Juice-PNG.png"
            alt=""
          />
        </div>

        <div class="top-products-content">
          <div class="top-products-text">
            <div class="top-products-title">Berry Juice</div>
            <div class="top-products-price">$ 7.5</div>
          </div>

          <i class="bx bxs-plus-circle bx-sm"></i>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="less">
h2 {
  font-weight: 400;
  margin: 10px 0;

}
.home {
  padding-bottom: 100px;
  .top-products-all{
    display: flex;
    overflow-y: auto;

  .top-products {
    margin-right: 10px;
    padding: 10px;
    border-radius: 10px;
    min-width: 120px;
    background-color: rgba(250, 248, 248);

    .top-products-img {
      img {
        width: 100px;
      }
    }

    .top-products-content {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    i {
      color: rgba(46, 154, 57);
    }
  }
}
  margin: 20px;
  .scroll-menu {
    .scroll-content {
      display: flex;
      overflow-y: auto;
      color: rgba(24, 24, 24);
      

      .avatar {

        background-color: rgba(250, 248, 248);
        padding: 10px;
        border-radius: 10px;
        margin: 2px;
        margin-right: 10px;
        margin-top: 20px;
        width: 70px;
        text-align: center;
        .title{
          font-weight: 600;
          font-size: 18px;
          margin-top: 5px;
        }
        i {
          color: rgba(255, 131, 62);
        }
      }
    }
  }
}
.header {
  margin-top: 40px;
  .combo-header {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
    border-radius: 10px;
    background-color: rgba(74, 174, 84);
    align-items: center;
    color: white;
    padding: 20px;
    .img {
      img {
        object-fit: cover;
        height: 70px;
      }
    }
    .text {
      width: 50%;
      h3 {
        font-weight: 400;
      }
      p {
        font-weight: 300;
      }
    }
  }
  .input {
    display: flex;
    position: relative;
    align-items: center;
    margin-top: 15px;
    input {
      width: 100%;
      background-color: rgba(250, 248, 248);
      border: 0;
      outline: none;
      padding: 10px;
      padding-left: 30px;
      border-radius: 10px;
    }
    .icon-input {
      position: absolute;

      margin-left: 5px;
    }
  }

  .title {
    font-weight: 350;
  }
}
</style>