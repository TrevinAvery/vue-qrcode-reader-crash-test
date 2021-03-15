# vue-qrcode-reader-crash-test

This is a simple repo intended to reproduce an error in [`vue-qrcode-reader`](https://github.com/gruhn/vue-qrcode-reader/issues/233).

I used `vue create` from `@vue/cli` to create it. Then I installed `vue-qrcode-reader` and replaced the `HellowWorld.vue` example component with a simple `QrcodeReader.vue` component that just loads the `QrcodeStream` and prints each decoded value to the console.

# Steps to reproduce

1. Launch the dev server with `npm run serve`

2. Connect your Android phone to your computer and navigate to `http://localhost:8080` in Chrome

3. Open `chrome://inspect/#devices` in Chrome and open the inspect window for the localhost tab so you can see the console and read the output of `QrcodeReader` and any errors

4. Start scanning qrcodes; anywhere from 10 to 70 scans, you will see an out of memory error, and the stream will stop scanning