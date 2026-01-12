<script lang="ts" setup>
import { useToast } from 'wot-design-uni'

defineOptions({
  name: 'Records',
  options: {
    virtualHost: true,
  },
})

const { show: showToast } = useToast()

definePage({
  style: {
    navigationBarTitleText: '%records.record%',
    navigationStyle: 'custom',
  },
})
</script>

<template>
  <view class="">
    <view>
      Test1
    </view>
    <wd-button>Primary Button</wd-button>
    <wd-button type="success">
      Success Button
    </wd-button>
    <wd-fab position="right-center">
      <wd-button
        custom-class="custom-button" type="primary"
        round @click="showToast('Triple Like')"
      >
        <wd-icon name="github-filled" size="22px" />
      </wd-button>
    </wd-fab>
  </view>
</template>

<style lang="scss" scoped>
//
</style>
