<template>
  <nav>
    <router-link to="/money" class="item" active-class="selected">
      <Icon name="money" />
      记账
    </router-link>
    <router-link to="/labels" class="item" active-class="selected">
      <Icon name="label" />
      标签
    </router-link>
    <router-link to="/statistics" class="item" active-class="selected">
      <Icon name="statistics" />
      统计
    </router-link>
  </nav>
</template>

<script lang="ts">
export default {
  name: 'Nav'
};
</script>

<style lang="scss" scoped>
@import "~@/assets/style/helper.scss";

nav {
  @extend %outerShadow;
  display: flex;
  flex-direction: row;
  font-size: 12px;

  >.item {
    padding: 2px 0;
    width: 33.33333%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    .icon {
      width: 32px;
      height: 32px;
    }

    .icon:hover {
      @-webkit-keyframes zy {
        10% {
          transform: rotate(15deg);
        }

        20% {
          transform: rotate(-10deg);
        }

        30% {
          transform: rotate(5deg);
        }

        40% {
          transform: rotate(-5deg);
        }

        50%,
        100% {
          transform: rotate(0deg);
        }
      }
    }
  }

  >.item :hover {
    background: rgb(25, 148, 131);
  }

  >.item.selected {
    color: #4e6ef2;
  }
}
</style>