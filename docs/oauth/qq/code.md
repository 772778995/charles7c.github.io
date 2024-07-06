---
layout: false
---
<script setup>
const params = new URLSearchParams(location.hash)
const access_token = params.get('#access_token')
const redirect_uri = params.get('state')
const redirectUrl = new URL(redirect_uri)
const redirectParams = new URLSearchParams(`?access_token=${access_token}`)
redirectUrl.search = redirectParams.toString()
console.log(redirectUrl)
window.href = redirectUrl.href
</script>