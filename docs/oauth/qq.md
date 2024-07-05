---
layout: false
---

<script setup>
const client_id = '102132332'
const response_type = 'token'
const redirect_uri = encodeURIComponent('https://wuhaochao.top/login')
const baseUrl = 'https://graph.qq.com/oauth2.0/authorize'
const url = `${baseUrl}?client_id=${client_id}&response_type=${response_type}&scope=all&redirect_uri=${redirect_uri}`
document.querySelector('html').addEventListener('click', () => {
  return window.open(
    url,
    'oauth2Login_10117',
    'height=525,width=685, toolbar=no, menubar=no, scrollbars=no, status=no, location=yes, resizable=yes'
  )
})
</script>

<style>
  /* 清空所有默认样式 */
body, h1, h2, h3, h4, h5, h6, p, ul, ol, li, a, img, div, span {
    margin: 0;
    padding: 0;
    border: 0;
    font-size: 100%;
    font: inherit;
    vertical-align: baseline;
}

/* 你可以在这里添加自定义样式 */
body {
    background-color: #fff;
    color: #000;
    font-family: Arial, sans-serif;
}
</style>