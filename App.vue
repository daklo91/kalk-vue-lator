<template>
  <view class="container">
    <view><text class="title">Kalk-Vue-Lator</text></view>
    <view class="result-container"
      ><text class="result-text">{{ result }}</text></view
    >
    <view class="button-container">
      <view class="button-sub-container"
        ><TouchableOpacity class="button-style">
          <Text class="button-text">7</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">8</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">9</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style button-color-gray">
          <Text class="button-text button-text-white">DEL</Text>
        </TouchableOpacity></view
      >
      <view class="button-sub-container"
        ><TouchableOpacity class="button-style">
          <Text class="button-text">4</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">5</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">6</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">+</Text>
        </TouchableOpacity></view
      >
      <view class="button-sub-container"
        ><TouchableOpacity class="button-style">
          <Text class="button-text">1</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">2</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">3</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">-</Text>
        </TouchableOpacity></view
      >
      <view class="button-sub-container"
        ><TouchableOpacity class="button-style">
          <Text class="button-text">.</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">0</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">/</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style">
          <Text class="button-text">x</Text>
        </TouchableOpacity></view
      >
      <view class="button-sub-container"
        ><TouchableOpacity class="button-style button-big button-color-gray">
          <Text class="button-text button-text-white">RESET</Text>
        </TouchableOpacity>
        <TouchableOpacity class="button-style button-big button-color-red">
          <Text class="button-text button-text-white">=</Text>
        </TouchableOpacity>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {
      message: "Hello World",
      result: 1337.355,
    };
  },
  methods: {
    exclaim() {
      this.message += "!";
    },
  },
};
</script>

<style>
.container {
  flex: 1;
  background-color: #3a4663;
  align-items: center;
  justify-content: flex-start;
  padding: 25px;
}
.title {
  margin-top: 70px;
  color: #fff;
  line-height: 35px;
  font-size: 32px;
}
.result-container {
  background-color: #181f33;
  border-radius: 10px;
  min-width: 100%;
  padding: 25px;
  margin-top: 32px;
  margin-left: 0;
  margin-right: 0;

}
.result-text {
  font-size: 32px;
  font-weight: 700;
  line-height: 36px;
  text-align: right;
  color: white;
}
.button-container {
  background-color: #242d44;
  border-radius: 10px;
  padding: 18px;
  margin-top: 24px;
  /* display: grid; */
}
.button-sub-container {
  flex: 1;
  flex-direction: row;
  justify-content: space-between;
  align-content: center;
  width: 100%;
  max-height: 74px;
}
.button-style {
  background-color: #eae3dc;
  height: 60px;
  width: 64px;
  margin: 7;
  flex: 1;
  align-items: center;
  justify-content: center;
  border-radius: 5px;
}
.button-big {
  width: 133px;
}
.button-text {
  color: #434a59;
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  line-height: 31px;
  text-align: center;
}
.button-text-white {
  color: #fff;
}
.button-color-red {
  background-color: #D03F2F;
}
.button-color-gray {
  background-color: #647198;
}
</style>
