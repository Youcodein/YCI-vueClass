<template>
  <section id="imageType" class="image__wrap" :class="attr">
    <h2>Why?</h2>
    <p>왜 사람들은 "다이어리 꾸미기" 에 열광하는가?</p>
    <div class="image__inner" :class="layout">
      <article class="image img1">
        <h3 class="image__title">Remember your Memories</h3>
        <p class="image__desc">
          기억으로 남기는 것도 좋은 방법이지만 기록으로 남기지 않은 기억은 금방
          휘발되는 법입니다. 멋진 기억들을 기록하고 이후에 펼쳐보면 많은
          감정들을 알려주죠.
        </p>
        <a class="image__btn" href="/" title="자세히 보기">자세히 보기</a>
      </article>
      <article class="image img2">
        <h3 class="image__title">See my Feelings</h3>
        <p class="image__desc">
          당신의 감정을 시각적으로 표현하고 싶지 않으신가요? 스티커를 붙이세요.
          그림을 그리세요. 당신의 추억을 장식하세요. 적절한 장식은 감정을
          실감나게 표현해줍니다. 마음에 드는 스티커나 그림으로 예쁘게
          장식해보세요
        </p>
        <a class="image__btn yellow" href="/" title="자세히 보기"
          >자세히 보기</a
        >
      </article>
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
<style>
/* imageType */
.image__inner {
  display: flex;
  justify-content: space-between;
}

.image {
  width: 49%;
  height: 370px;
  color: #fff;
  padding: 200px 30px 30px 30px;
  box-sizing: border-box;
}

.image.img1 {
  background: url(../../assets/img/image_bg01_01.jpg) no-repeat center;
}

.image.img2 {
  background: url(../../assets/img/image_bg01_02.jpg) no-repeat center;
}

.image__title {
  font-size: 32px;
  margin-bottom: 10px;
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

.image__desc {
  font-size: 16px;
  font-weight: 300;
  margin-bottom: 10px;
  line-height: 1.5;
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}

.image__btn {
  font-size: 16px;
  color: #fff;
  background-color: #b45a30;
  padding: 10px 20px;
  display: inline-block;
}

.image__btn.yellow {
  background-color: #b59140;
}

@media (max-width: 960px) {
}

@media (max-width: 600px) {
  .image__inner {
    flex-direction: column;
  }
  .image {
    width: 100%;
    padding: 210px 20px 20px 20px;
  }
  .image:first-child {
    margin-bottom: 20px;
  }
  .image__title {
    font-size: 24px;
  }
}

/* @media(max-width:1200px){
    #imageType{
        width: 96%;
        margin: 0 auto;
    }
    .image__inner.container{
        min-width: auto;
        width: auto;
    }

    .image__title{
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
    }
}

@media(max-width:600px){
    .image__inner{
        flex-wrap: wrap;
        justify-content: center;
    }
    .image{
        width: 96%;
        margin-bottom: 15px;
    }
    .image.img2{
        margin-bottom: 0;
    }
} */
</style>
