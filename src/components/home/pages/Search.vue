<template>
  <div :class="$style.search">
    <div :class="$style.wrapper">
      <div :class="$style.images">
        <div :class="$style.image">
          <img src="../../../assets/images/search/1.png" alt="" />
        </div>
        <div :class="$style.image">
          <img src="../../../assets/images/search/2.png" alt="" />
        </div>
        <div :class="$style.image">
          <img src="../../../assets/images/search/3.png" alt="" />
        </div>
        <div :class="$style.image">
          <img src="../../../assets/images/search/4.png" alt="" />
        </div>
        <div :class="$style.searchQuery">
          <svg-search :class="$style.searchQuerySvg" />
          <span :class="$style.searchQueryText"> простые блюда из курицы на ужин </span>
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
}

.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

.images {
}

.image {
}

.searchQuery {
  &Svg {
  }

  &Text {
  }
}

.description {
  height: 50%;
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
