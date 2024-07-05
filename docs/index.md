---
layout: home

title: Hocho的知识库
titleTemplate: 个人技术知识库，记录和分享个人碎片化、结构化、体系化的技术知识内容

hero:
  name: Hocho的知识库
  text: 专注 & 洞察 & 分享
  tagline: 个人技术知识库，记录 & 分享个人碎片化、结构化、体系化的技术知识内容。
  image:
    src: /logo.png
    alt: Logo
  actions:
    - theme: brand
      text: 快速开始
      link: /categories/issues/index
    - theme: alt
      text: 在 GitHub 查看
      link: https://github.com/772778995/charles7c.github.io

features:
  - icon:
      src: https://tool.hgs.cn/favicon.ico
    title: 嗨格
    details: 免费一键在线录屏，随时随地录制一切精彩！
    link: https://tool.hgs.cn
  - icon:
      src: https://www.iloveimg.com/img/favicons-img/favicon-32x32.png
    title: iLoveIMG
    details: 您可以批量编辑图像的所有工具，你的在线照片编辑器在这里，永远免费！
    link: https://www.iloveimg.com
  - icon:
      src: https://clipdrop.co/favicon.ico
    title: clipdrop
    details: 转为快速图像剪切与背景去除而设计（需科学上网）
    link: https://clipdrop.co
---
<script setup>
import $ from 'jquery'

const client_id = '102134934'
const response_type = 'token'
const redirect_uri = encodeURIComponent('https://wuhaochao.top/login')
const baseUrl = 'https://graph.qq.com/oauth2.0/authorize'
const url = `${baseUrl}?client_id=${client_id}&response_type=${response_type}&scope=all&redirect_uri=${redirect_uri}`

$('body').append($(`<img src="https://qzonestyle.gtimg.cn/qzone/vas/opensns/res/img/Connect_logo_7.png">`).css({ position: 'fixed', top: '20px', right: '120px', cursor: 'pointer' }).on('click', () => {
  window.open(
    url,
    'oauth2Login_10117',
    'height=525,width=685, toolbar=no, menubar=no, scrollbars=no, status=no, location=yes, resizable=yes'
  )
}))
</script>