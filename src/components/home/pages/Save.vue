<template>
  <div :class="$style.save">
    <div :class="$style.wrapper">
      <div :class="$style.description">
        <h1 :class="$style.descriptionTitle">Сохраняйте понравившиеся идеи</h1>
        <span :class="$style.descriptionText">
          Сохраняйте понравившиеся идеи, чтобы вернуться к ним в будущем.
        </span>
        <button :class="$style.descriptionButton">Просмотреть</button>
      </div>
      <div :class="$style.imagesWrapper">
        <div :class="$style.imagesBlockFirst">
          <img :class="$style.imageBackgroundBig" src="../../../assets/images/save/1.png" alt="" />
          <h5 :class="$style.imageDescriptionBig">Интерьер в стиле листа папоротника</h5>
          <div :class="$style.images">
            <img :class="$style.image" src="../../../assets/images/save/2.png" alt="" />
            <img :class="$style.image" src="../../../assets/images/save/3.png" alt="" />
            <img :class="$style.image" src="../../../assets/images/save/4.png" alt="" />
          </div>
        </div>
        <div :class="$style.imagesBlockSecond">
          <img :class="$style.imageBackground" src="../../../assets/images/save/5.png" alt="" />
          <h5 :class="$style.imageDescription">Спальня в скандинавском стиле</h5>
        </div>
        <div :class="$style.imagesBlockThird">
          <img
            :class="$style.imageBackgroundSmall"
            src="../../../assets/images/save/6.png"
            alt=""
          />
          <h5 :class="$style.imageDescriptionSmall">Балкон моей мечты</h5>
        </div>
        <div :class="$style.imagesBlockFourth">
          <img :class="$style.imageBackground" src="../../../assets/images/save/8.png" alt="" />
          <h5 :class="$style.imageDescription">Идеи для ванной комнаты</h5>
        </div>
        <div :class="$style.imagesBlockFifth">
          <img :class="$style.imageBackground" src="../../../assets/images/save/7.png" alt="" />
          <h5 :class="$style.imageDescription">Стильная подача напитков</h5>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

.save {
  height: 100vh;
  background: $background-save;
  padding: 85px 0 0 0;
}

.wrapper {
  display: grid;
  grid-template-columns: 1fr 1fr;
  height: 100vh;
}
.description {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  &Title {
    max-width: 100%;
    font-size: 60px;
    font-weight: bold;
    color: $save-text;
    text-align: center;
    line-height: 80px;
  }

  &Text {
    max-width: 375px;
    font-size: 24px;
    font-weight: 400;
    text-align: center;
    color: $save-text;
    margin: 16px 0 0 0;
  }

  &Button {
    height: 48px;
    min-width: 93px;
    background: $save-text;
    color: $background-save;
    font-size: 16px;
    text-align: center;
    font-weight: bold;
    margin: 24px 0 0 0;
    padding: 0 16px;
    border-radius: 99px;
  }
}

.imagesWrapper {
  position: relative;
  width: 100%;
  height: 100%;
  margin: 85px 0 0 0;
}

.imagesBlock {
  &First {
    position: absolute;
    top: 0px;
    left: 10px;
  }

  &Second {
    position: absolute;
    top: 0px;
    left: 464px;
  }

  &Third {
    position: absolute;
    top: 280px;
    left: 447px;
  }

  &Fourth {
    position: absolute;
    top: 500px;
    left: 429px;
  }

  &Fifth {
    position: absolute;
    top: 460px;
    left: 159px;
  }
}

.imageBackground {
  width: 223px;
  height: 235px;
  object-fit: cover;
  border-radius: 32px;

  &Big {
    width: 400px;
    height: 420px;
    object-fit: cover;
    border-radius: 32px;
  }

  &Small {
    width: 165px;
    height: 173px;
    object-fit: cover;
    border-radius: 16px;
  }
}

.imageDescription {
  position: absolute;
  bottom: 0;
  padding: 24px;
  color: $text-white;
  font-weight: 500;
  font-size: 28px;
  line-height: 38px;

  &Big {
    position: absolute;
    top: 15%;
    color: $text-white;
    font-weight: 500;
    font-size: 56px;
    margin: 0 0 0 40px;
    line-height: 80px;
  }

  &Small {
    position: absolute;
    bottom: 0;
    padding: 0 22px 24px 16px;
    color: $text-white;
    font-weight: 500;
    font-size: 20px;
    line-height: 28px;
  }
}

.images {
  display: flex;
  position: absolute;
  top: 300px;
  left: 40px;
}

.image {
  width: 90px;
  height: 130px;
  margin: 0 4px;
  object-fit: cover;
}
</style>
