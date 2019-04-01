    # vue-touch-simple #
    **使用方法：**
    ```<div>
        <p>-1- 安装 npm install vue-touch-simple -S</p>
        <p>-2- main.js中 </p>
        <p>   import Touch from 'vue-touch-simple'</p>
        <p>   Vue.use(Touch) //use一下（前提引入先Vue）</p>
        <p>-3- 代码中示例</p>
    </div>```

       ```
		<template>
            <div>
                <ul>
                    <li v-touch:swipeleft="swipeLeft">swipeLeft</li>
                    <li v-touch:swiperight="swipeRight">swipeLeft</li>
                    <li v-touch:swipeup="swipeUp">swipeLeft</li>
                    <li v-touch:swipedown="swipeDown">swipeLeft</li>
                    <li v-touch:longpress="longpress">lonePress</li>
                </ul>
            </div>
        </template>
        <script>
        export default {
            methods:{
                swipeLeft(el,binding){
                    alert('swipeLeft')
                },
                swipeRight(el,binding){
                    alert('swipeRight')
                },
                swipeUp(el,binding){
                    alert('swipeUp')
                },
                swipeDown(el,binding){
                    alert('swipeDown')
                },
                longpress(el,binding){
                    alert('longpress')
                }
            }
        }
        </script>
		```
