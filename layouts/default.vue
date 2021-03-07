<template>
  <div>
    <a-page-header
    style="border: 1px solid rgb(235, 237, 240)"
    title="ประวัติการเข้า-ออกประตูภาคไฟฟ้า"
    @back="() => null"
  />
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
.ant-page-header-ghost {
  background-color: #576b9e;
}
.ant-page-header-heading-title{
    color: #fff;
  }

</style>
