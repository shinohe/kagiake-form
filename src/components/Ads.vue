<template>
 <div ref="ads" class="ad">
   <iframe ref="adsIframe">

   </iframe>
 </div>
</template>

<script>
import isMobile from 'ismobilejs'

export default {
  async mounted () {
    const iframe = this.$refs.adsIframe
    iframe.frameBorder = 0
    iframe.marginHeight = 0
    iframe.marginWidth = 0
    this.$refs.ads.appendChild(iframe)
    const PC_HTML = '<body><script src="https://adm.shinobi.jp/s/4c74b446a2ef7b0643f0bc384b21b143"><\/script><\/body>'
    const SMART_HTML = '<body><script src="https://adm.shinobi.jp/s/66cdeaab5412f8bc5b5724987c0834f9"><\/script><\/body>'

    const iframeDocument = iframe.contentWindow.document
    iframeDocument.open()
    if (this.isPC()) {
      iframeDocument.write(PC_HTML)
    } else {
      iframeDocument.write(SMART_HTML)
    }
    iframeDocument.close()
  },
  methods: {
    isPC () {
      if (isMobile.phone) {
        return true
      }
      return false
    }
  }
}
</script>
<style scoped>
.ad{
    width:300px;
    height:250px;
    margin: 0 auto;
}
.ad iframe{
    top:0;
    left:0;
    width:100%;
    height:100%;
}
</style>
