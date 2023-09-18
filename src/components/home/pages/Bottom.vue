<template>
  <div :class="$style.bottom">
    <div :class="$style.backgroundImages">
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/1.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/2.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/3.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/4.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/5.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/6.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/7.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/8.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/9.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/10.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/11.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/12.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/13.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/14.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/15.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/16.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/17.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/18.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/19.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/20.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/21.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/22.jpg" alt="" />
      </div>
      <div :class="$style.backgroundImage">
        <img :class="$style.backgroundImage" src="../../../assets/images/bottom/23.jpg" alt="" />
      </div>
    </div>
    <div :class="$style.wrapper">
      <div :class="$style.description">
        <h1 :class="$style.descriptionTitle">Зарегистрируйтесь, чтобы находить больше идей</h1>
      </div>
      <div :class="$style.wrapperRegistration">
        <div :class="$style.registration">
          <div :class="$style.registrationLogo">
            <img :class="$style.authorizationLogo" src="../../../assets/icons/logo.svg" alt="" />
          </div>
          <div :class="$style.registrationWelcome">
            <h2 :class="$style.authorizationWelcome">Добро пожаловать в Pinterest</h2>
          </div>
          <div :class="$style.registrationDecription">
            <h5 :class="$style.authorizationDecription">Находите новые идеи для вдохновения</h5>
          </div>
          <div :class="$style.registrationForm">
            <form :class="$style.form" action="">
              <div :class="$style.formMail">
                <label :class="$style.formMailLabel" for="email"> Адрес электронной почты </label>
                <input :class="$style.formMailInput" type="email" name="email" id="" />
              </div>
              <div :class="$style.formPassword">
                <label :class="$style.formPasswordLabel" for="password"> Пароль </label>
                <input :class="$style.formPasswordInput" type="password" name="password" id="" />
              </div>
              <div :class="$style.formBirth">
                <label :class="$style.formBirthLabel" for="date"> Дата рождения </label>
                <input :class="$style.formBirthInput" type="date" name="date" id="" />
              </div>
              <div :class="$style.formButton">
                <button :class="$style.formButtonСontinue">Продолжить</button>
              </div>
            </form>
            <span :class="$style.registrationFormText"> ИЛИ </span>
            <div :class="$style.registrationFormSocial">
              <button :class="$style.registrationFormSocialFacebook">Продолжить</button>
              <button :class="$style.registrationFormSocialGoogle">Продолжить</button>
            </div>
          </div>
          <div :class="$style.registrationAgreement">
            <span :class="$style.registrationAgreementText">
              Продолжая, вы соглашаетесь с положениями основных документов Pinterest. Это
              <a :class="$style.registrationAgreementLink" href="">Условия предоставления услуг</a>
              и
              <a :class="$style.registrationAgreementLink" href="">Политика конфиденциальности</a>.
              А также подтверждаете, что прочли их.
              <a :class="$style.registrationAgreementLink" href="">Уведомление.</a>
            </span>
          </div>
          <div :class="$style.registrationLogin">
            <span :class="$style.registrationLoginText">
              Уже зарегистрировались? <a :class="$style.registrationLoginLink" href="">Войти</a>
            </span>
          </div>
          <div :class="$style.registrationBusiness">
            <button :class="$style.registrationBusinessButton">
              Создать бесплатный бизнес-аккаунт
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" module>
@import '@/assets/scss/_variables.scss';

.bottom {
}
</style>
