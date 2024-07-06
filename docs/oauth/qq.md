---
layout: false
---

<script setup>
const client_id = '102134934'
const response_type = 'code'
const redirect_uri = encodeURIComponent('https://wuhaochao.top/oauth/qq/code')
const baseUrl = 'https://graph.qq.com/oauth2.0/authorize'
const state = new URLSearchParams(location.search).get('redirect_url')
const url = `${baseUrl}?client_id=${client_id}&response_type=${response_type}&scope=all&state=${state}&redirect_uri=${redirect_uri}`
location.href = url
</script>