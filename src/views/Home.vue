<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <form action="/quotes" method="POST">
      <input type="text" placeholder="name" name="name">
      <input type="text" placeholder="quote" name="quote">
      <button type="submit">Submit</button>
    </form>
  </div>
</template>

<script src="https://cdn.onesignal.com/sdks/OneSignalSDK.js" async=""></script>
<script>
  var OneSignal = window.OneSignal || [];
    OneSignal.push(function () {
      OneSignal.init({
        appId: "${5f57b1e3-c137-424d-ace8-71d6b6efb87f}",
        autoRegister: false,
        notifyButton: {
          enable: true,
        },
      });
    });
</script>
<script>

// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  },
  methods:{

  }
}
</script>
