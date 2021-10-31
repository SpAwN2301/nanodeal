<template>
  <div class="offers">
    <div class="offers__sticky">
      <div class="offers__head">
        <h2 class="offers__title">Предложения</h2>
        <div class="offers__right-wrapper">
          <div class="offers__search">
            <Search />
          </div>
          <div class="offers__profile">
            <Profile />
          </div>
        </div>
      </div>
      <div class="offers__tabs-scroll">
        <div class="offers__tabs">
          <div
            id="tabActive"
            @click="showProducts('tabActive')"
            class="offers__tab active"
          >
            <div class="offers__tab-icon">
              <svg
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M10 0V1.93548C12.1388 1.93548 14.1901 2.78514 15.7025 4.29753C17.2149 5.80992 18.0645 7.86116 18.0645 10C18.0645 12.1388 17.2149 14.1901 15.7025 15.7025C14.1901 17.2149 12.1388 18.0645 10 18.0645V20C12.6522 20 15.1957 18.9464 17.0711 17.0711C18.9464 15.1957 20 12.6522 20 10C20 7.34784 18.9464 4.8043 17.0711 2.92893C15.1957 1.05357 12.6522 0 10 0Z"
                  fill="#00C667"
                />
                <path
                  d="M6.32084 1.77307C6.58807 2.23593 6.42948 2.82779 5.96662 3.09503C5.50375 3.36226 4.91189 3.20367 4.64466 2.74081C4.37742 2.27795 4.53601 1.68609 4.99888 1.41885C5.46174 1.15162 6.0536 1.31021 6.32084 1.77307Z"
                  fill="#00C667"
                />
                <path
                  d="M3.09503 5.96887C3.36226 5.506 3.20367 4.91414 2.74081 4.64691C2.27795 4.37967 1.68609 4.53826 1.41885 5.00112C1.15162 5.46399 1.31021 6.05585 1.77307 6.32308C2.23593 6.59032 2.82779 6.43173 3.09503 5.96887Z"
                  fill="#00C667"
                />
                <path
                  d="M0.967742 10.9677C1.50221 10.9677 1.93548 10.5345 1.93548 10C1.93548 9.46553 1.50221 9.03226 0.967742 9.03226C0.433273 9.03226 0 9.46553 0 10C0 10.5345 0.433273 10.9677 0.967742 10.9677Z"
                  fill="#00C667"
                />
                <path
                  d="M6.32052 18.2268C6.58775 17.7639 6.42917 17.172 5.9663 16.9048C5.50344 16.6376 4.91158 16.7962 4.64434 17.259C4.37711 17.7219 4.5357 18.3138 4.99856 18.581C5.46142 18.8482 6.05329 18.6896 6.32052 18.2268Z"
                  fill="#00C667"
                />
                <path
                  d="M3.09503 14.0308C3.36226 14.4937 3.20367 15.0855 2.74081 15.3528C2.27795 15.62 1.68609 15.4614 1.41885 14.9986C1.15162 14.5357 1.31021 13.9438 1.77307 13.6766C2.23593 13.4094 2.82779 13.568 3.09503 14.0308Z"
                  fill="#00C667"
                />
                <path
                  d="M8.70964 11.2129L13.1871 6.73545L14.5548 8.10319L9.39351 13.2645C9.21206 13.4457 8.96609 13.5475 8.70964 13.5475C8.45319 13.5475 8.20722 13.4457 8.02577 13.2645L5.12254 10.3613L6.49028 8.99351L8.70964 11.2129Z"
                  fill="#00C667"
                />
              </svg>
            </div>
            <p class="offers__tab-name">Активные</p>
          </div>
          <div
            id="tabModer"
            @click="showProducts('tabModer')"
            class="offers__tab"
          >
            <div class="offers__tab-icon">
              <svg
                width="20"
                height="20"
                viewBox="0 0 20 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M10.6021 9.39899H14.5093C15.0065 9.39899 15.411 9.80354 15.411 10.3007C15.411 10.5417 15.3172 10.768 15.1468 10.9378C14.9764 11.1082 14.7501 11.202 14.5093 11.202H9.70049C9.20337 11.202 8.79883 10.7975 8.79883 10.3004V5.4915C8.79883 4.99439 9.20337 4.58984 9.70049 4.58984C9.94153 4.58984 10.1678 4.68392 10.3383 4.85403C10.5084 5.02444 10.6021 5.25106 10.6021 5.4918V9.39899Z"
                  fill="#2C98F0"
                />
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M6.10694 0.786547C7.34101 0.264486 8.65082 0 10 0C11.3492 0 12.6593 0.264486 13.8931 0.786547C15.0842 1.29027 16.1532 2.0113 17.0711 2.92889C17.989 3.84648 18.7097 4.91584 19.2135 6.10694C19.7355 7.34101 20 8.65082 20 10C20 11.3492 19.7355 12.659 19.2135 13.8931C18.7097 15.0842 17.9887 16.1532 17.0711 17.0711C16.1535 17.989 15.0842 18.7097 13.8931 19.2135C12.6593 19.7352 11.3492 20 10 20C8.65082 20 7.34101 19.7352 6.10694 19.2135C4.91615 18.7097 3.84678 17.9887 2.92889 17.0711C2.011 16.1535 1.29027 15.0842 0.786547 13.8931C0.264787 12.659 0 11.3495 0 10C0 8.65052 0.264787 7.34071 0.786547 6.10694C1.29027 4.91584 2.0113 3.84648 2.92889 2.92889C3.84648 2.0113 4.91615 1.29027 6.10694 0.786547ZM18.1967 10C18.1967 5.47337 14.5269 1.80332 10 1.80332C5.47307 1.80332 1.80332 5.47367 1.80332 10.0003C1.80332 14.5269 5.47307 18.197 10 18.197C14.5269 18.197 18.197 14.5269 18.1967 10Z"
                  fill="#2C98F0"
                />
              </svg>
            </div>
            <p class="offers__tab-name">На модерации</p>
          </div>
          <div
            id="tabDraft"
            @click="showProducts('tabDraft')"
            class="offers__tab"
          >
            <div class="offers__tab-icon">
              <svg
                width="18"
                height="18"
                viewBox="0 0 18 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M9.37587 1.39348L13.6391 5.65742L14.1629 5.13365C15.3601 3.93672 15.2849 1.99176 14.1629 0.869706C12.9663 -0.326858 11.021 -0.252347 9.89891 0.869706L9.37587 1.39348Z"
                  fill="#FE8862"
                />
                <path
                  d="M17.2302 16.5039H0.773468C0.39945 16.5039 0.0254326 16.8031 0.0254326 17.252C0.0254326 17.5347 0.143774 17.7578 0.343931 17.8846C0.39945 17.9196 0.460812 17.9474 0.528019 17.9668C0.60326 17.9887 0.685806 18 0.773468 18H17.2302C17.6788 18 17.9783 17.7009 17.9783 17.252C17.9783 17.0273 17.903 16.84 17.7723 16.7092C17.6415 16.5784 17.4545 16.5039 17.2302 16.5039Z"
                  fill="#FE8862"
                />
                <path
                  d="M8.32687 2.48813L12.5587 6.71957L6.68762 12.5906L2.45582 8.35919L8.32687 2.48813Z"
                  fill="#FE8862"
                />
                <path
                  d="M0.249697 14.8581C0.39945 15.0079 0.698225 15.0827 0.997732 15.0079L5.48594 13.5118L1.67126 9.69674L0.0999432 14.1101C0.0239716 14.2237 0.00570869 14.3566 0.0349293 14.4892C0.0641499 14.6185 0.13866 14.7474 0.249697 14.8581Z"
                  fill="#FE8862"
                />
              </svg>
            </div>
            <p class="offers__tab-name">Черновики</p>
          </div>
          <div
            id="tabArchive"
            @click="showProducts('tabArchive')"
            class="offers__tab"
          >
            <div class="offers__tab-icon">
              <svg
                width="22"
                height="18"
                viewBox="0 0 22 18"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M2.91687 0H19.0832C20.3316 0 21.3472 1.01558 21.3472 2.26403V5.40748C21.3472 5.66527 21.1372 5.87526 20.8794 5.87526H20V15.736C20 16.9844 18.9844 18 17.736 18H4.26406C3.01561 18 2.00003 16.9844 2.00003 15.736V5.87526H1.12061C0.937056 5.87526 0.779391 5.76907 0.702924 5.61771C0.670657 5.55401 0.652832 5.48236 0.652832 5.40748V2.26403C0.652832 1.01558 1.66842 0 2.91687 0ZM17.736 16.1663C17.9731 16.1663 18.1663 15.973 18.1663 15.736V5.87526H3.8337V15.736C3.8337 15.973 4.02698 16.1663 4.26406 16.1663H17.736ZM14.6113 9C14.6113 9.25779 14.4013 9.46778 14.1435 9.46778H7.85657C7.59878 9.46778 7.3888 9.25779 7.3888 9V8.10187C7.3888 7.84408 7.59878 7.6341 7.85657 7.6341H14.1435C14.4013 7.6341 14.6113 7.84408 14.6113 8.10187V9ZM2.24327 2.26403C2.24327 2.0657 2.32944 1.88711 2.46627 1.76377C2.58577 1.65611 2.74386 1.59044 2.91687 1.59044H19.0832C19.4546 1.59044 19.7568 1.8927 19.7568 2.26403V4.28482H2.24327V2.26403Z"
                  fill="#9A99B8"
                />
              </svg>
            </div>
            <p class="offers__tab-name">Архив</p>
          </div>
        </div>
      </div>
    </div>

    <div class="offers__products-wrapper">
      <Search />
      <ul class="offers__products" :class="{ active: activeClass }">
        <li v-for="(product, index) in productsToShow" :key="index">
          <ProductCard
            :status="product.status"
            :mission="product.mission"
            :present="product.present"
          />
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import ProductCard from "./ProductCard.vue";
import Search from "./Search.vue";
import Profile from "./Profile.vue";

export default {
  name: "Offers",
  components: {
    ProductCard,
    Search,
    Profile,
  },

  data() {
    return {
      activeClass: false,
      productsToShow: [],
      products: [
        {
          status: "Активное",
          img: "../assets/ProductCard/desk/logo.webp",
          mission: "Записать сторис в кросcовках Nike Air Max 720",
          present: "Репост строис в официальном аккаунте NikeRussia",
        },
        {
          status: "Активное",
          img: "../assets/ProductCard/desk/logo.webp",
          mission: "Опубликовать сторис в Инстаграм со словами «Just Do It»",
          present: "10% скидка в интернет-магазине",
        },
        {
          status: "Модерация",
          img: "../assets/ProductCard/desk/logo.webp",
          mission: "Опубликовать сторис в Инстаграм со словами «Just Do It»",
          present: "10% скидка в интернет-магазине",
        },
        {
          status: "Черновик",
          img: "../assets/ProductCard/desk/logo.webp",
          mission: "Опубликовать сторис в Инстаграм со словами «Just Do It»",
          present: "10% скидка в интернет-магазине",
        },
      ],
    };
  },

  methods: {
    primaryRender() {
      this.activeClass = true;
      setTimeout(() => {
        this.activeClass = false;
      }, 500);
      this.products.forEach((product) => {
        if (product.status === "Активное") {
          this.productsToShow.push(product);
        }
      });
    },
    showProducts(activeTabId) {
      const tabPrev = document.querySelector(".offers__tab.active");
      const tabCur = document.querySelector(`#${activeTabId}`);

      this.activeClass = true;
      setTimeout(() => {
        this.activeClass = false;
      }, 500);
      this.productsToShow.length = 0;
      tabPrev.classList.remove("active");
      tabCur.classList.add("active");

      switch (activeTabId) {
        case "tabActive":
          this.products.forEach((product) => {
            if (product.status === "Активное") {
              this.productsToShow.push(product);
            }
          });
          break;
        case "tabModer":
          this.products.forEach((product) => {
            if (product.status === "Модерация") {
              this.productsToShow.push(product);
            }
          });
          break;
        case "tabDraft":
          this.products.forEach((product) => {
            if (product.status === "Черновик") {
              this.productsToShow.push(product);
            }
          });
          break;
        case "tabArchive":
          this.products.forEach((product) => {
            if (product.status === "Архив") {
              this.productsToShow.push(product);
            }
          });
          break;
        default:
          break;
      }
    },
  },

  beforeMount() {
    this.primaryRender();
  },
};
</script>

<style scoped>
.offers {
  overflow-x: hidden;
  overflow-y: auto;

  width: 80%;
  height: 100%;

  background: #faf5f2;
  border: 6px solid rgba(39, 41, 49, 0.07);
  border-radius: 20px;
}
.offers::-webkit-scrollbar {
  display: none;
}

.offers__sticky {
  position: sticky;
  top: 0;

  padding: 35px 30px 0;

  background: #faf5f2;
  border-bottom: 0.5px solid #d9c4b7;
}
.offers__head {
  display: flex;
  justify-content: space-between;
  align-items: center;

  margin-bottom: 27px;
}
.offers__title {
  font-family: "Raleway";
  font-style: normal;
  font-weight: bold;
  font-size: 24px;

  color: #2d3134;
}
.offers__right-wrapper {
  display: flex;
  column-gap: 20px;
}
.offers__tabs-scroll {
  overflow: auto;
}
.offers__tabs-scroll::-webkit-scrollbar {
  display: none;
}
.offers__tabs {
  margin-bottom: 25px;
  display: flex;
  align-items: center;

  column-gap: 20px;

  width: max-content;
}
.offers__tab {
  transition: 0.5s;
  cursor: pointer;
  padding: 10px 14px;

  display: flex;
  align-items: center;
  column-gap: 8px;

  border-radius: 10px;
}
.offers__tab.active {
  pointer-events: none;
  transition: 0.5s;
  background: #ffffff;
}
.offers__tab-icon {
  pointer-events: none;
}
.offers__tab-icon > svg {
  vertical-align: top;
}
.offers__tab-name {
  pointer-events: none;
  font-family: "Raleway";
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  text-align: center;

  color: #2d3134;
}

.offers__products {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 343px));
  gap: 39px;

  justify-content: space-around;

  padding: 30px;
}
.offers__products.active {
  animation: fadeIn 0.5s;
  animation-fill-mode: forwards;
}

.offers__products-wrapper > .search {
  display: none;
}
@media screen and (max-width: 768px) {
  .offers {
    width: 100%;
    border-width: 4px;
  }

  .offers__sticky {
    padding: 30px 16px 0;
    position: unset;
  }
  .offers__head {
    justify-content: center;
    margin-bottom: 25px;
  }
  .offers__title {
    font-size: 5.3305vw;
  }
  .offers__right-wrapper {
    display: none;
  }

  .offers__tabs {
    margin-bottom: 16px;
  }

  .offers__products-wrapper {
    padding: 16px;
  }
  .offers__products {
    padding: 20px 0;
    gap: 25px;
  }

  .offers__products-wrapper > .search {
    display: block;

    max-width: unset;
    width: 100%;
  }
}
</style>
