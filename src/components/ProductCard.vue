<template>
  <div class="productCard">
    <div class="productCard__head">
      <div class="productCard__logo">
        <div class="productCard__logo-img">
          <img src="../assets/ProductCard/desk/logo.webp" alt="" />
        </div>
        <p class="productCard__logo-name">Nike</p>
      </div>
      <div class="productCard__status">{{ status }}</div>
    </div>

    <div class="productCard__img">
      <img src="../assets/ProductCard/desk/product1.webp" alt="" />
    </div>

    <div class="productCard__container20">
      <p class="productCard__mission">{{ mission }}</p>

      <div class="productCard__present">
        <div class="productCard__present-icon">
          <img src="../assets/ProductCard/desk/gift.webp" alt="" />
        </div>
        <p class="productCard__present-text">{{ present }}</p>
      </div>

      <ul class="productCard__list">
        <li class="productCard__list-item">
          <p>Новые сообщения</p>
          <div class="productCard__count-wrapper">
            <div class="productCard__count productCard__count_red">22</div>
            <div class="productCard__count-arrow">
              <img src="../assets/ProductCard/desk/next.webp" alt="" />
            </div>
          </div>
        </li>
        <li class="productCard__list-item">
          <p>Новые заявки</p>
          <div class="productCard__count-wrapper">
            <div class="productCard__count productCard__count_grey">2</div>
            <div class="productCard__count-arrow">
              <img src="../assets/ProductCard/desk/next.webp" alt="" />
            </div>
          </div>
        </li>
        <li class="productCard__list-item">
          <p>До завершения</p>
          <div class="productCard__count-wrapper">
            <div class="productCard__count productCard__count_orange">
              1н: 2д: 23ч: 20м: 10с
            </div>
          </div>
        </li>
        <li class="productCard__list-item">
          <p>Выполнено</p>
          <div class="productCard__count-wrapper">
            <div class="productCard__count productCard__count_green">
              250 / 3 000
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "ProductCard",
  props: {
    status: String,
    mission: String,
    present: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.productCard {
  padding: 14px;

  max-width: 343px;
  background: #ffffff;
  box-shadow: 0px 10px 20px rgba(233, 216, 207, 0.3);
  border-radius: 4px 20px 20px 20px;
}

.productCard__head {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.productCard__logo {
  display: flex;
  align-items: center;
  column-gap: 13px;
}
.productCard__logo-img {
  width: 36px;
  height: 36px;
}
.productCard__logo-img > img {
  width: 100%;
  height: auto;
}
.productCard__logo-name {
  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  /* Graphite */

  color: #272931;
}

.productCard__status {
  display: grid;
  place-content: center;
  width: 90px;
  height: 30px;

  background: rgba(0, 198, 103, 0.08);
  border-radius: 8px;

  font-family: "Raleway";
  font-style: normal;
  font-weight: 600;
  font-size: 13px;

  color: #00c667;
}

.productCard__img {
  margin-top: 10px;
  margin-bottom: 20px;

  width: 100%;
  height: auto;
}
.productCard__img > img {
  width: 100%;
  height: auto;
}

.productCard__container20 {
  padding: 0 6px;
}
.productCard__mission {
  display: flex;
  align-items: center;

  margin-bottom: 10px;

  height: 2.375em;

  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 19px;

  color: #272931;
}

.productCard__present {
  display: flex;
  align-items: center;
  column-gap: 10.38px;

  margin-bottom: 14px;

  height: 2em;
}
.productCard__present-icon {
  width: 17.62px;
  height: 18px;
}
.productCard__present-icon > img {
  width: 100%;
  height: auto;
}
.productCard__present-text {
  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;
  /* Pink */

  color: #fc5a8b;
}

.productCard__list-item {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 50px;

  border-top: 0.5px solid #d4d8e3;
}
.productCard__list-item > p {
  font-family: Raleway;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 16px;
  /* Graphite */

  color: #272931;
}

.productCard__count-wrapper {
  display: flex;
  align-items: center;
  column-gap: 5px;
}
.productCard__count-arrow {
  cursor: pointer;
  width: 16px;
  height: 16px;
}
.productCard__count-arrow > img {
  width: 100%;
  height: auto;
}
.productCard__count {
  display: grid;
  place-content: center;
}
.productCard__count.productCard__count_red {
  width: 30px;
  height: 30px;

  border-radius: 50%;
  background: #f93c47;

  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;

  color: #ffffff;
}
.productCard__count.productCard__count_grey {
  width: 30px;
  height: 30px;

  border-radius: 50%;
  background: #f7f7fa;
  border: 2.5px solid #ffffff;

  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;

  color: #9a99b8;
}
.productCard__count.productCard__count_orange {
  width: 170px;
  height: 30px;

  background: rgba(254, 136, 98, 0.08);
  border-radius: 8px;

  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 15px;

  color: #fe8862;
}
.productCard__count.productCard__count_green {
  width: 110px;
  height: 30px;

  background: #00c667;
  border-radius: 8px;

  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 14px;
  line-height: 16px;

  color: #ffffff;
}
</style>
