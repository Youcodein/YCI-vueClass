<template>
  <section id="textType" class="text__wrap scroll" :class="attr">
    <span>My Tip</span>
    <h2 class="mb70">๐๋๋ง์ ๋ค์ด์ด๋ฆฌ ๊พธ๋ฏธ๊ธฐ ํ!๐</h2>
    <div class="text__inner" :class="layout">
      <div class="text t1">
        <h3 class="text__title">Only Text</h3>
        <p class="text__desc">
          ๋ฌธ์๋ง์ ๋งค๋ ฅ์ด ์์ง์. ์ด๋ ํ ๊ธฐ๊ต๋, ์ฅ์๋ ์๋ ํ์คํธ๋ง์ ๋งค๋ ฅ์
          ๋ฏธ๋๋ฉ๋ฆฌ์ฆ์ ์๋ฆ๋ค์์ ์ฐ์ํฉ๋๋ค.
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
      <div class="text t2">
        <h3 class="text__title">Handwriting</h3>
        <p class="text__desc">
          ๊ธ์๋ง์ผ๋ก  ๋๋ฌด ๋ฐ๋ฐํ์ ๊ฐ์? ๊ทธ๋ ๋ค๋ฉด ๊ธ์จ์ ์์ ์ ์ธ ๊ฐ๊ฐ์ ๋ํด๋ณด๋ฉด
          ์ด๋จ๊น์? ํฌ์ธํธ๊ฐ ๋  ๊ฑฐ์์!
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
      <div class="text t3">
        <h3 class="text__title">Color</h3>
        <p class="text__desc">
          ๋ฌด์ฑ์์ ๋ค์ด์ด๋ฆฌ๋ ๋ฉ์ง์ง๋ง ๋น์ ์ ๊ธฐ์ต์ ์์ ์น ํด๋ณด๋๊ฑด ์ด๋ ์ธ์?
          ๋น์ ์ ๊ฐ์ ์ ์๊น๋ก ํํํด๋ณด์ธ์!
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
      <div class="text t4">
        <h3 class="text__title">Hand Drawing</h3>
        <p class="text__desc">
          ๊ธ๋ง์ผ๋ก๋ ํํํ๊ธฐ ์ด๋ ค์ธ ๋, ๊ทธ๋ฆผ์ ๋ํด๋ณด์ธ์! ๋น์ ๋ ์ ๋ ๋ฌด์์ธ์ง
          ์ดํดํ๊ธฐ ์ฌ์์! ๋ฌผ๋ก , ์ดํดํ๊ธฐ ์ด๋ ค์ด ๊ทธ๋ฆผ๋ ๋งค๋ ฅ์ ์ด์ฃ !
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
      <div class="text t5">
        <h3 class="text__title">Sticker</h3>
        <p class="text__desc">
          ๊ทธ๋ฆผ์ ์์ ์ด ์๋ค๋ฉด ์ด๋ฏธ ๋ง๋ค์ด์ง ๊ทธ๋ฆผ์ ํ์ฉํด๋ด์. ๊ทธ๋์, ๋ฐ๋ก
          ์คํฐ์ปค๋ฅผ ์ด์ฉํด๋ณด์ธ์!
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
      <div class="text t6">
        <h3 class="text__title">Just WRITING!</h3>
        <p class="text__desc">
          ์์ ํ์ ๋ชจ๋ ์์ด๋ฒ๋ฆฌ์ธ์! ์์ ๋ค์ด ๋ค์ด์ด๋ฆฌ๋ฅผ ์ํ์๋์? ๊ทธ๋ผ
          ๊ฒ๋จน์ง ๋ง๊ณ  ์ผ๋จ "์ฐ์ธ์!"
        </p>
        <a href="/" class="text__btn">๋๋ณด๊ธฐ</a>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: {
    attr: String,
    layout: String,
  },
};
</script>
<style scoped>
/* textType */
.text__inner {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}

.text {
  width: 32%;
  margin-bottom: 2%;
  padding: 20px;
  box-sizing: border-box;
  border-radius: 10px;
  transition: background 0.4s;
}

.text:hover {
  background: #f5f5f5;
}

.text__title {
  font-size: 24px;
  line-height: 1;
  margin-bottom: 10px;
  white-space: nowrap;
  text-overflow: ellipsis;
  position: relative;
  padding-top: 75px;
}

.text__title::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 60px;
  height: 60px;
  border-radius: 50%;
  background: url(../../assets/img/text_icon1.svg);
}

.text.t1 .text__title::before {
  background-position: 0 0;
}

.text.t2 .text__title::before {
  background-position: -60px 0;
}

.text.t3 .text__title::before {
  background-position: -120px 0;
}

.text.t4 .text__title::before {
  background-position: -180px 0;
}

.text.t5 .text__title::before {
  background-position: -240px 0;
}

.text.t6 .text__title::before {
  background-position: -300px 0;
}

.text__desc {
  font-size: 18px;
  font-weight: 300;
  line-height: 1.4;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  color: #666;
  margin-bottom: 20px;
}

.text__btn {
  font-size: 16px;
  line-height: 1;
  text-decoration: underline;
  text-underline-position: under;
  color: #666;
}

@media (max-width: 960px) {
  .text {
    width: 49%;
    background: #f5f5f5;
  }
}

@media (max-width: 600px) {
  .text__title {
    font-size: 20px;
  }
  .text__desc {
    font-size: 16px;
  }
}
@media (max-width: 480px) {
  .text {
    width: 100%;
  }
}
</style>
