<template>
  <div>
    <button type="button" class="button buttonDisable">click mi</button>
  </div>
</template>
<script>
export default {
  data () {
    return {
    }
  },
  methods: {
  }
}
</script>
<style lang="less">
@import '../style/variables';
@import '../style/StyleAll';
.button {
  width: 99px;
  height: 44px;
  border-radius: 22px;
  background: linear-gradient(180deg, #bc9cff 0%, #8ba4F9 100%);
  border: none;
  .fontSize12;
  color: white;
}
.buttonDisable {
  opacity: .5;
}
</style>
