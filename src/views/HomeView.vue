<script setup>

</script>

<template>
  <div>
    <div class="max-w-1440">
      <div class="section grid" data-aos="fade-up" data-aos-duration="3000">
        <p class="font-white title">Never transcribe manually again</p>
        <p class="content">
          Tanscribe clips from any Avid Media Composer project with ease. Say goodbye to the hassle of exporting to
          Quicktimes or uploading clips one-by-one to a subpar prosumer tool.
          Made for professionals, by professionals.
        </p>
        <div class="section_center">
          <div class="mailinput">
            <input placeholder="Enter your email" />
            <button>Request Beta Access</button>
          </div>
        </div>
      </div>
      <div class="section  section_2">
        <img data-aos="zoom-in" data-aos-duration="3000" src="../assets/images/section2.png" alt="image" />
      </div>
      <div class="section  section_3" data-aos="fade-down" data-aos-easing="linear" data-aos-duration="1500">
        <p>EdMon speeds up your transcribing, searching and pre-editing of video, saving you hours of work.</p>
        <div class="watch_btn_t">
          <a id="play-video" class="video-play-button" href="#">
            <span></span>
          </a>
          <h2>Watch video</h2>
        </div>
      </div>
      <div class="section  card even section_4">
        <img data-aos="flip-left" src="../assets/images/Maskgroup(1).png" alt="Mask group (1)" />
        <div data-aos="fade-left">
          <h3>Batch transcribe</h3>
          <p>With just a few clicks, you can open an Avid project file, select the clips you want to transcribe, and in
            minutes, you/'ll have fully transcribed text available on our cloud-based platform.</p>
        </div>

      </div>
      <div class="section  card odd section_5">
        <div data-aos="fade-right">
          <h3>Online access</h3>
          <p>The transcribed video is stored on our cloud platform, accessible from anywhere and organized in a way that
            matches your Media Composer project.</p>
        </div>
        <img data-aos="flip-right" src="../assets/images/Maskgroup(2).png" alt="Mask group(1)" />
      </div>
      <div class="section  card even section_6">
        <img data-aos="flip-left" src="../assets/images/Maskgroup(3).png" alt="Mask group(1)" />
        <div data-aos="fade-left">
          <h3>Text based editing</h3>
          <p>Browse through the text, pick and choose the parts you want, and add them to a rough cut. The process of
            editing is now faster and more efficient, allowing you to search and select in text instead of video.
            Finally,
            export your selections as an AAF file and seamlessly integrate them back into Media Composer.</p>
        </div>

      </div>
      <div class="section  card odd section_7">
        <div data-aos="fade-right">
          <h3>Roundtrip from MC to EdMon (and back)</h3>
          <p>Enjoy the convenience of editing a rough cut in text instead of video, and send your final product back to
            Media Composer for fine-tuning. With our AAF exports, you'll be able to link back to your original Media
            Composer clips instantly.</p>
        </div>
        <img data-aos="flip-right" src="../assets/images/Maskgroup(4).png" alt="Mask group (1)" />
      </div>
    </div>
    <div class="section learn">
      <h1 data-aos="fade-up" data-aos-anchor-placement="top-center">Less pain - more editing.</h1>
      <p data-aos="fade-right" data-aos-duration="1000">
        EdMon is a professional tool specifically designed for Avid editors. It can transcribe multiple video files in
        one go, created for editors who need to transcribe large volumes of video content (like hours of interviews
        for a documentary).</p>
      <br />
      <p data-aos="fade-left" data-aos-duration="1000">In short, EdMon is the ideal solution for Avid editors who need
        to transcribe large amounts of video content
        quickly and efficiently. Less pain - more editing.

      </p>
      <div class="section_center">
        <div class="mailinput">
          <input placeholder="Enter your email" />
          <button>Request Beta Access</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.grid {
  display: grid;
}

.section .title {
  text-align: center;
  font-family: var(--font-main);
  font-style: normal;
  font-weight: 600;
  font-size: 100px;
  margin: 100px 106px;
  line-height: 121px;
}

.content {
  margin: 10px 349px;
  font-family: var(--font-main);
  font-style: normal;
  font-weight: 400;
  font-size: 24px;
  line-height: 141.52%;
  text-align: center;
  letter-spacing: 0.04em;

  color: #C0C0C0;
}

.section_center {
  display: flex;
  justify-content: center;
}

.mailinput {
  margin-top: 35px;
  display: flex;
  width: 660px;
  height: 64px;
  box-sizing: border-box;
  background: #fff0;
  border: 0.5px solid #FFFFFF;
  border-radius: 32px;
  align-items: center;
  justify-content: space-between;
  line-height: 22px;
  padding-left: 32px;
  color: #A8A8A8;
}

.mailinput button {
  box-sizing: border-box;
  width: 235px;
  height: 54px;
  color: #424242;
  border: 0.5px solid #FFFFFF;
  border-radius: 32px;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 22px;
  margin-right: 5px;
  cursor: pointer;
}

.mailinput input {
  background-color: #fff0;
  font-family: var(--font-main);
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  width: 350px;
  height: 40px;
}

.section_2 {
  background-size: cover;
  height: 868px;
  min-height: 470px;
  background-image: url('../assets/images/section2_bg.png');
}


.section_3 {
  background-size: cover;
  height: 770px;
  background-image: url('../assets/images/section3_bg.png');
}

.section_3 p {
  max-width: 928px;
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  line-height: 141.52%;
  text-align: center;
  letter-spacing: 0.04em;

  color: #E0E0E0;
}

.watch_btn_t {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 24px;
  margin-top: 42px;
}

.watch_btn_t h2 {
  padding-left: 32px;

}

.card {
  flex-direction: row;
  background-repeat: no-repeat;
  background-position: center;
  border-radius: 12px;
}

.section_4 {
  background-image: url('../assets/images/section4_bg.png');
}

.even img {
  padding-left: 120px;
}

.section_5 {
  background-image: url('../assets/images/section5_bg.png');
}

.odd img {
  padding-right: 122px;
}

.section_6 {
  background-image: url('../assets/images/section6_bg.png');
}


.section_7 {
  background-image: url('../assets/images/section7_bg.png');
}

.card div {
  max-width: 268px;
  margin: 32px 94px 0 108px;
}

.card div p {
  margin-top: 32px;
  font-size: 18px;
  color: #F1F1F1;
}

.card div h3 {
  font-size: 32px;
  color: #E0E0E0;
}

.learn {
  width: 100%;
  max-width: initial;
  background: linear-gradient(180deg, rgba(0, 0, 0, 0)0%, rgba(29, 52, 254, 0.224) 134.17%);
}

.learn h1 {
  font-weight: 700;
  font-size: 80px;
  line-height: 141.52%;
  /* or 113px */
  margin: 13px;
  max-width: 928px;
  text-align: center;
  letter-spacing: 0.04em;

  color: #FFFFFF;
}

.learn p {
  max-width: 928px;
  font-weight: 400;
  font-size: 24px;
  line-height: 141.52%;
  /* or 34px */

  text-align: center;

  color: #FFFFFF;
}

@media (max-width: 1200px) {
  .section.grid {
    text-align: left;
  }

  .content {
    margin: 50px;
  }

  .section .title {
    font-size: 4.8rem;
    font-style: normal;
    font-weight: 600;
    letter-spacing: -.03em;
    line-height: 1.1;
  }

  .section_2 img {
    width: 90%;
  }

  .card img {
    width: 40%;
    min-width: 162px;
  }

  img {
    padding: 0 !important;
  }
}

@media (max-width: 768px) {

  .section_2 {
    display: grid;
    align-items: center;
    justify-content: center;
    justify-items: center;
    align-content: center;
    height: auto;
  }

  .section .title {
    font-weight: 600;
    font-size: 40px;
  }

  .content {
    margin: auto;
    max-width: 321px;
    margin-top: 0;
  }


  .section.grid p {
    text-align: left;
    max-width: 358px;
    margin-bottom: 0;
  }

  .watch_btn_t h2 {
    padding-left: 16px;

  }

  .section_3 {
    display: flex;
    align-items: flex-start;
    height: 232px;
  }

  .section_3 p {
    text-align: left;
    margin-left: 7%;
    margin-top: 41px;
    font-size: 18px;
    max-width: 323px;
  }

  .watch_btn_t {
    margin-left: 7%;
    font-size: 16px;
  }





  .mailinput {
    width: 90%;
    min-width: 359px;
    height: 48px;
    padding-left: 16px;
  }

  .mailinput input {
    width: 180px;
  }

  .mailinput button {
    width: 174px;
    font-weight: 500;
    font-size: 14px;
    line-height: 17px;
    height: 37px;
  }

  .learn h1 {
    width: 358px;
    height: 96px;
    text-align: left;
    font-family: 'Inter';
    font-style: normal;
    font-weight: 600;
    font-size: 40px;
    line-height: 48px;
    margin-left: 16px;
    color: #FFFFFF;
  }

  .learn p {
    margin-left: 16px;
    font-size: 16px;
  }

  .section.learn.grid {
    height: auto !important;
  }

  .section.learn.grid .section_center {
    margin-bottom: 100px;
  }



}

@media (max-width: 648px) {
  .section .title {
    margin-left: 16px;
    margin-right: 16px;
  }

  .mailinput input {
    width: 164px;
  }
}

@media (max-width: 500px) {
  .card div {
    max-width: 375px;
    margin: 0;
    margin-left: 19px;
  }

  .card div h3 {
    margin-top: 20px;
    font-size: 18px;
    font-style: normal;
    font-weight: 500;
    line-height: 141.52%;
    /* or 25px */
    max-width: 164px;
    letter-spacing: 0.04em;
  }

  .card div p {
    margin-top: 16px;
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 17px;
    max-width: 153px
  }

  .section_4 {
    background-image: url('../assets/images/mobileCard.png');
    height: 228px;
    margin-bottom: 40px;
  }



  .section_5 {
    background-image: url('../assets/images/mobileCard1.png');
    height: 208px;
    margin-bottom: 40px;
  }


  .section_6 {
    background-image: url('../assets/images/mobileCard2.png');
    height: 346px;
    margin-bottom: 40px;
  }


  .section_7 {
    background-image: url('../assets/images/mobileCard3.png');
    height: 333px;
    margin-bottom: 40px;
  }
}
</style>