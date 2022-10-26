<template>
  <section id="sliderType" class="slider__wrap nexon scroll">
    <h2 class="ir">Hot Issue</h2>
    <div class="slider__inner">
      <div class="slider">
        <div class="slider__img">
          <div class="desc">
            <span>Dairy</span>
            <h3>Art of Dairy</h3>
            <p>
              다이어리는 이제 기록을 넘어선 문화 예술이 되었습니다.<br />
              다이어리 꾸미기의 매력에 빠져보세요
            </p>
            <div class="btn">
              <a href="#">자세히보기</a>
              <a href="#" class="black">사이트보기</a>
            </div>
          </div>
        </div>
        <div class="slider__arrow">
          <a href="#" class="left"><span class="ir">이전 이미지</span></a>
          <a href="#" class="right"><span class="ir">다음 이미지</span></a>
        </div>
        <div class="slider__dot">
          <a href="#" class="dot active"><span class="ir">1</span></a>
          <a href="#" class="dot"><span class="ir">2</span></a>
          <a href="#" class="dot"><span class="ir">3</span></a>
          <a href="#" class="play"><span class="ir">플레이</span></a>
          <a href="#" class="stop"><span class="ir">정지</span></a>
        </div>
      </div>

      <!-- <div class="swiper mySwiper">
                    <div class="swiper-wrapper">
                        <div class="swiper-slide">
                            <div class="desc">
                                <span>Dairy</span>
                                <h3>Art of Dairy</h3>
                                <p>
                                    다이어리는 이제 기록을 넘어선 문화 예술이 되었습니다.<br>
                                    다이어리 꾸미기의 매력에 빠져보세요
                                </p>
                                <div class="btn">
                                    <a href="#">자세히보기</a>
                                    <a href="#" class="black">사이트보기</a>
                                </div>
                            </div>
                        </div>
                        <div class="swiper-slide">
                            <div class="desc">
                                <span>Dairy</span>
                                <h3>Art of Dairy</h3>
                                <p>
                                    다이어리는 이제 기록을 넘어선 문화 예술이 되었습니다.<br>
                                    다이어리 꾸미기의 매력에 빠져보세요
                                </p>
                                <div class="btn">
                                    <a href="#">자세히보기</a>
                                    <a href="#" class="black">사이트보기</a>
                                </div>
                            </div>
                        </div>
                        <div class="swiper-slide">
                            <div class="desc">
                                <span>Dairy</span>
                                <h3>Art of Dairy</h3>
                                <p>
                                    다이어리는 이제 기록을 넘어선 문화 예술이 되었습니다.<br>
                                    다이어리 꾸미기의 매력에 빠져보세요
                                </p>
                                <div class="btn">
                                    <a href="#">자세히보기</a>
                                    <a href="#" class="black">사이트보기</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="swiper-pagination"></div>
                    <div class="swiper-button">
                        <div class="swiper-button-play"><span class="ir">play</span></div>
                        <div class="swiper-button-stop"><span class="ir">stop</span></div>
                    </div>
                    <div class="swiper-button-next"></div>
                    <div class="swiper-button-prev"></div>

                </div> -->
    </div>
  </section>
</template>

<style scope>
.slider__inner {
  margin-top: 70px;
}

.slider {
}

.slider__img {
  background: url(../../assets/img/slider_bg01.jpg) no-repeat center / cover;
}

.slider__img .desc {
  width: 1160px;
  margin: 0 auto;
  padding: 100px 20px;
}

.slider__img .desc span {
  font-size: 16px;
  background-color: #fff;
  padding: 1px 14px 0 14px;
  text-transform: uppercase;
  margin-bottom: 10px;
  display: inline-block;
  border-radius: 30px;
}

.slider__img .desc h3 {
  font-size: 110px;
  font-weight: 300;
  line-height: 1;
  color: #fff;
  text-transform: uppercase;
  margin-bottom: 16px;
  margin-left: -8px;
}

.slider__img .desc p {
  font-size: 20px;
  font-weight: 300;
  color: #fff;
  line-height: 1.45;
  margin-bottom: 130px;
}

.slider__img .desc .btn {
}

.slider__img .desc .btn a {
  font-size: 16px;
  background-color: #fff;
  padding: 11px 50px;
  display: inline-block;
}

.slider__img .desc .btn a.black {
  background-color: #000;
  color: #fff;
}

.slider {
  position: relative;
}

.slider__arrow {
}

.slider__arrow a {
  position: absolute;
  top: 50%;
  width: 30px;
  height: 56px;
  background-image: url(../../assets/img/slider_icon.svg);
  transform: translateY(-50%);
}

.slider__arrow a.left {
  left: 20px;
}

.slider__arrow a.right {
  right: 20px;
  background-position: -50px 0;
}

.slider__dot {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  bottom: 25px;
}

.slider__dot a {
  display: inline-block;
  width: 16px;
  height: 16px;
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -20px -70px;
}

.slider__dot a.active {
  background-position: 0 -70px;
}

.slider__dot a.play {
  background-position: -40px -70px;
}

.slider__dot a.stop {
  background-position: -60px -70px;
}

/* swiper */
.swiper-slide {
  background: url(../../assets/img/slider_bg01.jpg) no-repeat center / cover;
}

.swiper-slide .desc {
  /* width: 1160px; */
  width: 100%;
  margin: 0 auto;
  padding: 100px 100px;
  box-sizing: border-box;
}

.swiper-slide .desc span {
  font-size: 16px;
  background-color: #fff;
  padding: 1px 14px 0 14px;
  text-transform: uppercase;
  margin-bottom: 10px;
  display: inline-block;
  border-radius: 30px;
}

.swiper-slide .desc h3 {
  font-size: 110px;
  font-weight: 300;
  line-height: 1;
  color: #fff;
  text-transform: uppercase;
  margin-bottom: 16px;
  margin-left: -8px;
}

.swiper-slide .desc p {
  font-size: 20px;
  font-weight: 300;
  color: #fff;
  line-height: 1.45;
  margin-bottom: 130px;
}

.swiper-slide .desc .btn {
}

.swiper-slide .desc .btn a {
  font-size: 16px;
  background-color: #fff;
  padding: 11px 50px;
  display: inline-block;
}

.swiper-slide .desc .btn a.black {
  background-color: #000;
  color: #fff;
}

.swiper-button-next,
.swiper-button-prev {
  width: 30px !important;
  height: 56px !important;
  background-image: url(../../assets/img/slider_icon.svg);
}

.swiper-button-next {
  background-position: -50px 0;
}

.swiper-button-next::after,
.swiper-button-prev::after {
  opacity: 0;
}

.swiper-pagination-bullet {
  width: 16px !important;
  height: 16px !important;
  background-image: url(../../assets/img/slider_icon.svg) !important;
  background-color: transparent !important;
  opacity: 1 !important;
  background-position: -20px -70px !important;
}

.swiper-pagination-bullet-active {
  background-position: 0 -70px !important;
}

.swiper-button {
  position: absolute;
  margin-left: 40px;
  left: 50%;
  bottom: 24px;
  z-index: 1000;
  display: flex;
  cursor: pointer;
}
.swiper-button-stop {
  width: 16px;
  height: 16px;
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -40px -70px;
}
.swiper-button-play {
  width: 16px;
  height: 16px;
  background-image: url(../../assets/img/slider_icon.svg);
  background-position: -40px -70px;
}

@media (max-width: 960px) {
  .swiper-slide .desc {
    text-align: center;
  }
  .swiper-slide .desc h3 {
    font-size: 70px;
  }
}

@media (max-width: 600px) {
  .swiper-slide .desc {
    padding: 80px 0;
  }
  .swiper-slide .desc h3 {
    font-size: 40px;
  }

  .swiper-slide .desc p {
    font-size: 16px;
    margin-bottom: 50px;
  }

  .swiper-slide .desc .btn a {
    padding: 10px 25px;
  }
}
</style>
