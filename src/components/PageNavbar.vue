<template>
    <nav class="navbar">
        <ul>
            <li>
                <router-link to="/">首頁</router-link>
            </li>
            <li>
                <router-link to="/about">作品集</router-link>
            </li>
            <li>
                <router-link to="/about">部落格</router-link>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss">
.navbar {
    position: fixed;
    top: 0%;
    left: 0%;
    right: 0%;
    background-color: rgba(184, 184, 184, 0.205);
    backdrop-filter: blur(0.5rem);
    z-index: 5;
    &>ul {
        display: flex;
        gap: 1rem;
        padding-top: 0.5rem;
        padding-bottom: 0.5rem;
        &>li {
            list-style-type: none;
            &>a {
                color: #e0e2e9;
                text-decoration-line: none;
            }   
        }
    }
}
</style>