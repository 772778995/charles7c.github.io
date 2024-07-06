---
layout: false
---
<script setup>
const params = new URLSearchParams(location.search)
alert(params.get('code))
</script>