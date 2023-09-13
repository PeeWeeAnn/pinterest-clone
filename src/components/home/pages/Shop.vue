<template>
  <div :class="$style.shop">
    <div :class="$style.wrapper">
      <div :class="$style.imagesWrapper">
        <div :class="$style.imageBackground">
          <img
            :class="$style.imageBackground"
            src="../../../assets/images/shop/background.png"
            alt=""
          />
        </div>
        <div :class="$style.story">
          <div :class="$style.storyImages">
            <img :class="$style.storyImage" src="../../../assets/images/shop/story.png" alt="" />
            <img :class="$style.storyAvatar" src="../../../assets/images/shop/avatar.png" alt="" />
          </div>
          <div :class="$style.storyDescription">
            <span :class="$style.storyDescriptionName">Scout the City</span>
            <span :class="$style.storyDescriptionSubscribers">56,7 тыс. подписчиков</span>
          </div>
        </div>
      </div>
      <div :class="$style.description">
        <h1 :class="$style.descriptionTitle">Просмотрите, сделайте, опробуйте и примерьте</h1>
        <span :class="$style.descriptionText">
          В Pinterest вы можете находить для себя новые увлечения и идеи со всего мира.
        </span>
        <button :class="$style.descriptionButton">Просмотреть</button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

.shop {
  height: 100vh;
  background: $background-shop;
}

.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
  height: 100vh;
}

.imagesWrapper {
  position: relative;
  width: 100%;
  height: 100%;
}

.imageBackground {
  object-fit: cover;
  height: 100vh;
  width: 960px;
}

.story {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  position: absolute;
  bottom: 96px;
  left: 84px;

  &Images {
    position: relative;
  }

  &Image {
    width: 215px;
    height: 383px;
    border-radius: 16px;
  }

  &Avatar {
    position: absolute;
    left: -36px;
    bottom: -36px;
    width: 96px;
  }

  &Description {
    width: 125px;
    margin: 0 0 0 48px;
    display: flex;
    flex-direction: column;

    &Name {
      color: $text-white;
    }

    &Subscribers {
      color: $text-white;
      font-weight: 400;
    }
  }
}

.description {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &Title {
    max-width: 420px;
    font-size: 60px;
    font-weight: bold;
    color: $shop-text;
    text-align: center;
    line-height: 80px;
  }

  &Text {
    max-width: 420px;
    font-size: 24px;
    font-weight: 400;
    text-align: center;
    color: $shop-text;
    margin: 16px 0 0 0;
  }

  &Button {
    height: 48px;
    min-width: 93px;
    background: $shop-text;
    color: $background-shop;
    font-size: 16px;
    text-align: center;
    font-weight: bold;
    margin: 24px 0 0 0;
    padding: 0 16px;
    border-radius: 99px;
  }
}
</style>
