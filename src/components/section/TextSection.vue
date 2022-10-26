<template>
  <section id="textType" class="text__wrap scroll" :class="attr">
    <span>My Tip</span>
    <h2 class="mb70">📖나만의 다이어리 꾸미기 팁!🖋</h2>
    <div class="text__inner" :class="layout">
      <div class="text t1">
        <h3 class="text__title">Only Text</h3>
        <p class="text__desc">
          문자만의 매력이 있지요. 어떠한 기교도, 장식도 없는 텍스트만의 매력은
          미니멀리즘의 아름다움을 연상합니다.
        </p>
        <a href="/" class="text__btn">더보기</a>
      </div>
      <div class="text t2">
        <h3 class="text__title">Handwriting</h3>
        <p class="text__desc">
          글자만으론 너무 밋밋하신가요? 그렇다면 글씨에 예술적인 감각을 더해보면
          어떨까요? 포인트가 될 거예요!
        </p>
        <a href="/" class="text__btn">더보기</a>
      </div>
      <div class="text t3">
        <h3 class="text__title">Color</h3>
        <p class="text__desc">
          무채색의 다이어리도 멋지지만 당신의 기억에 색을 칠해보는건 어떠세요?
          당신의 감정을 색깔로 표현해보세요!
        </p>
        <a href="/" class="text__btn">더보기</a>
      </div>
      <div class="text t4">
        <h3 class="text__title">Hand Drawing</h3>
        <p class="text__desc">
          글만으로는 표현하기 어려울 때, 그림을 더해보세요! 당신도 저도 무엇인지
          이해하기 쉬워요! 물론, 이해하기 어려운 그림도 매력적이죠!
        </p>
        <a href="/" class="text__btn">더보기</a>
      </div>
      <div class="text t5">
        <h3 class="text__title">Sticker</h3>
        <p class="text__desc">
          그림에 자신이 없다면 이미 만들어진 그림을 활용해봐요. 그래요, 바로
          스티커를 이용해보세요!
        </p>
        <a href="/" class="text__btn">더보기</a>
      </div>
      <div class="text t6">
        <h3 class="text__title">Just WRITING!</h3>
        <p class="text__desc">
          앞의 팁은 모두 잊어버리세요! 자신다운 다이어리를 원하시나요? 그럼
          겁먹지 말고 일단 "쓰세요!"
        </p>
        <a href="/" class="text__btn">더보기</a>
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
