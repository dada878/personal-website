<template>
    <section class="about">
        <h1>關於</h1>
        <p>{{greeting}}我是一個人類</p>
        <p>擅長網頁前端開發與 Python 實作專案</p>
        <p>正在學習各種演算法與資料結構</p>
        <p>這是使用 Vue 建立的網站</p>
        <p>未來希望可以在這裡放更多文章和作品</p>
    </section>
</template>
<script lang="ts" setup>

import { ref } from "vue";

const greeting = ref("");

const currentHour = new Date().getHours();

if (currentHour < 12) {
    greeting.value = "早安";
} else if (currentHour < 18) {
    greeting.value = "中安";
} else {
    greeting.value = "晚安";
}

</script>
<style lang="scss" scoped>
.about {
    padding-bottom: 2rem;
}
</style>