---
layout: false
---

<script setup>
const client_id = '102132332'
const response_type = 'token'
const redirect_uri = encodeURIComponent('https://wuhaochao.top/oauth/qq/code')
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