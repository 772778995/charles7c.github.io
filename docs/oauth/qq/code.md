---
layout: false
---
<script setup>
const params = new URLSearchParams(location.hash)
const token = params.get('#access_token')
const state = params.get('state')
console.log(location.hash, params, token, state)
open(`https://graph.qq.com/oauth2.0/me?access_token=${token}&fmt=json`)
</script>