<template>
  <div class="ReviewContainer">
    <div class="ReviewColumnLeft">
      <img src="../assets/insert_emoticon-24px.svg" class="ReviewImg">
      <div class="ReviewLike">
      <LikeButton/>
      </div>
    </div>
    <div class="ReviewColumnRight">
      <p class="ReviewTitle ReviewTitleBold">Мурад Сарафанов</p>
      <p class="ReviewTitle">{{this.reviewData}} дней назад</p>
      <p class='ReviewTitle ReviewText'>Великолепный матрас на кровати в основной спальне! А пуфик вообще потрясающий. И стены,
        действительно, шумоподавляющие. Выкрикивал комплименты повару — никто не жаловался из соседей.</p>
    </div>
  </div>
</template>
<script>
import LikeButton from '../components/LikeButton'
export default {
  components: {
    LikeButton
  },
  data () {
    return {
      reviewData: 5
    }
  }
}
</script>
<style lang="less">
@import '../style/variables';
@import '../style/StyleAll';
.ReviewContainer {
  display: flex;
  justify-content: space-between;
}
.ReviewColumnLeft {
  width: 48px;
  margin-right: 10px;
}
.ReviewTitle {
  .fontSize14;
  opacity: .75;
}
.ReviewTitleBold {
  font-weight: bold;
}
.ReviewText {
  width: 653px;
  margin-top: 10px;
   @media (max-width: 1000px) {
     width: 320px;
  }
   @media (max-width: 380px) {
     width: 265px;
  }
  }

.ReviewImg {
  width: 48px;
  height: 48px;
  margin-bottom: 10px;
}
.ReviewLike {
  padding-left: 4px;
}
</style>
