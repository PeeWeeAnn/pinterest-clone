<template>
  <div :class="$style.search">
    <div :class="$style.wrapper">
      <div :class="$style.imagesWrapper">
        <div :class="$style.images">
          <div :class="$style.image">
            <img :class="$style.imageFirst" src="../../../assets/images/search/1.png" alt="" />
          </div>
          <div :class="$style.image">
            <img :class="$style.imageSecond" src="../../../assets/images/search/2.png" alt="" />
          </div>
          <div :class="$style.image">
            <img :class="$style.imageThird" src="../../../assets/images/search/3.png" alt="" />
          </div>
          <div :class="$style.image">
            <img :class="$style.imageFourth" src="../../../assets/images/search/4.png" alt="" />
          </div>
          <div :class="$style.searchQuery">
            <svg-search :class="$style.searchQuerySvg" />
            <h5 :class="$style.searchQueryText">простые блюда из курицы на ужин</h5>
          </div>
        </div>
      </div>
      <div :class="$style.description">
        <h1 :class="$style.descriptionTitle">Найдите идею</h1>
        <span :class="$style.descriptionText">
          Что еще вы хотите опробовать? Придумайте запрос на интересующую тему, например «простые
          блюда из курицы на ужин», и просмотрите результаты.
        </span>
        <button :class="$style.descriptionButton">Просмотреть</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import SvgSearch from '@/assets/icons/search.svg?component'
</script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

.search {
  height: 100vh;
  background: $background-search;
  padding: 85px 0 0 0;
}

.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
  height: 83vh;
}

.imagesWrapper {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}

.images {
  width: 537px;
  height: 611px;
  border-radius: 16px;
  position: relative;

  :nth-child(1) {
    top: 88px;
    left: 148px;
    z-index: 5;
  }

  :nth-child(2) {
    top: 0px;
    right: 15px;
  }

  :nth-child(3) {
    top: 150px;
    left: 0px;
  }

  :nth-child(4) {
    right: 0px;
    top: 353px;
  }
}

.image {
  position: absolute;
  object-fit: cover;

  &First {
    width: 298px;
    height: 456px;
    border-radius: 16px;
  }

  &Second {
    width: 178px;
    height: 218px;
    border-radius: 16px;
  }

  &Third {
    width: 204px;
    height: 285px;
    border-radius: 16px;
  }

  &Fourth {
    width: 164px;
    height: 258px;
    border-radius: 16px;
  }
}

.searchQuery {
  position: absolute;
  height: 100px;
  width: 316px;
  top: 231px;
  left: 103px;
  background: $background-white;
  z-index: 10;
  display: flex;
  align-items: center;
  border-radius: 999px;

  &Svg {
    width: 32px;
    height: 32px;
  }

  &Text {
    color: #6e0f3c;
    font-size: 24px;
    font-weight: bold;
    text-align: center;
  }
}

.description {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &Title {
    font-size: 60px;
    font-weight: bold;
    color: $search-text;
  }

  &Text {
    max-width: 400px;
    font-size: 24px;
    font-weight: 400;
    text-align: center;
    color: $search-text;
    margin: 16px 0 0 0;
  }

  &Button {
    height: 48px;
    min-width: 93px;
    background: $search-text;
    color: $background-search;
    font-size: 16px;
    text-align: center;
    font-weight: bold;
    margin: 24px 0 0 0;
    padding: 0 16px;
    border-radius: 99px;
  }
}
</style>
