---
layout: false
---
<script setup>
const params = new URLSearchParams(location.hash)
const access_token = params.get('#access_token')
const redirect_uri = params.get('state')
location.href = redirect_uri + `?access_token=${access_token}`
</script>