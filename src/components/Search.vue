<template>
  <div class="search">
    <input type="text" class="search__input" placeholder="Поиск" />

    <button class="search__button">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="17"
        height="16"
        viewBox="0 0 17 16"
        fill="none"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M13.2962 13.996C11.8854 15.2431 10.0311 16 8 16C3.58172 16 0 12.4183 0 8C0 3.58172 3.58172 0 8 0C12.4183 0 16 3.58172 16 8C16 9.68621 15.4783 11.2506 14.5875 12.5405C14.6293 12.5707 14.6693 12.6046 14.7069 12.6423L16.2469 14.1822C16.6287 14.5641 16.6287 15.1832 16.2469 15.565C15.865 15.9469 15.2459 15.9469 14.8641 15.565L13.3241 14.0251C13.3146 14.0155 13.3053 14.0058 13.2962 13.996ZM14.0444 8C14.0444 11.3383 11.3383 14.0444 8 14.0444C4.66175 14.0444 1.95556 11.3383 1.95556 8C1.95556 4.66175 4.66175 1.95556 8 1.95556C11.3383 1.95556 14.0444 4.66175 14.0444 8Z"
          fill="#9A99B8"
        />
      </svg>
    </button>
  </div>
</template>

<script>
export default {
  name: "Search",
  props: {},
};
</script>

<style scoped>
.search {
  max-width: 250px;
  height: 36px;

  position: relative;
  display: flex;
}
.search__input {
  padding: 10px;
  padding-left: 38px;

  width: 100%;

  border: none;
  border-radius: 13px;
  outline: none;
  font-size: 20px;
  color: #2d3134;
  background: #ffffff;
}
.search__input::placeholder {
    font-family: "Raleway";
    font-style: normal;
    font-weight: 600;
    font-size: 14px;

    color: #9A99B8;
}
.search__button {
  position: absolute;
  left: 10px;
  top: calc(50% - 8px);

  display: grid;
  place-content: center;

  width: 16.5px;
  height: 16px;

  border: none;
  background: transparent;
  cursor: pointer;
}
</style>
