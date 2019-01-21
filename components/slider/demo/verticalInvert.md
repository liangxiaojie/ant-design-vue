<cn>
#### 反向垂直
反向垂直方向的 Slider。
</cn>

<us>
#### Invert Vertical
The invert vertical Slider.
</us>

```html
<template>
  <div style="height: 300px">
    <div style="float:left;height: 300px;marginLeft: 70px">
      <a-slider vertical verticalInvert :defaultValue="30" />
    </div>
    <div style="float:left;height: 300px;marginLeft: 70px">
      <a-slider vertical verticalInvert range :step="10" :defaultValue="[20, 50]" />
    </div>
    <div style="float:left;height: 300px;marginLeft: 70px">
      <a-slider vertical verticalInvert range :marks="marks" :defaultValue="[20, 60]" />
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      marks: {
        0: '0',
        20: '20%',
        40: '40%',
        60: '60%',
        80: '80%',
        100: {
          style: {
            color: '#f50',
          },
          label: <strong>100%</strong>,
        },
      },
    }
  },
  methods: {
    handleDisabledChange(disabled) {
      this.disabled = disabled
    }
  },
}
</script>
<style scoped>
.code-box-demo .ant-slider {
  margin-bottom: 16px;
}
</style>
```

