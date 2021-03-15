<template>
  <qrcode-stream @decode="onDecode"></qrcode-stream>
</template>

<script>
import { QrcodeStream } from 'vue-qrcode-reader'

export default {
  name: 'QrcodeReader',
  components: {
    QrcodeStream
  },
  methods: {
    onDecode(result) {
      console.log(result)
    }
  }
}
</script>
