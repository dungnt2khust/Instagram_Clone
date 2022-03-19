<template>
  <div class="search position-relative">
    <Icon_Search
      v-if="!focusSearch"
      class="search__icon--search position-absolute"
    />
    <input
      type="text"
      placeholder="Search"
      class="search__input w-100 p-v-3 p-r-16"
      :class="{ 'p-l-16': focusSearch, 'p-l-32': !focusSearch }"
      v-on="inputListeners"
    />
  </div>
</template>

<script>
import Icon_Search from "../Icons/Icon_Search";
export default {
  name: "Search",
  components: {
    Icon_Search,
  },
  data() {
    return {
      focusSearch: false,
    };
  },
  computed: {
    inputListeners() {
      return Object.assign({}, this.$listeners, {
        focus: () => {
          console.log("focus");
          this.focusSearch = true;
        },
        blur: () => {
          console.log("blur");
          this.focusSearch = false;
        },
        input: () => {
          console.log("input");
        },
      });
    },
  },
};
</script>

<style lang="scss">
.search {
  flex: 1;
  max-width: 268px;
  .search__icon--search {
    top: 50%;
    left: 10px;
    transform: translateY(-50%);
  }
  .search__icon--cancel {
  }
  .search__input {
    outline: none;
    border: none;
    background-color: #efefef;
    height: 36px;
    border-radius: 8px;
    width: 200px;
    box-sizing: border-box;
    &::-webkit-input-placeholder,
    &:-ms-input-placeholder,
    &::placeholder {
      /* Edge */
      color: red;
    }
  }
}
</style>