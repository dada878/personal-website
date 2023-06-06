<template>
    <nav class="navbar">
        <ul>
            <li>
                <router-link to="/">首頁</router-link>
            </li>
            <li>
                <router-link to="/projects">作品集</router-link>
            </li>
            <li>
                <router-link to="/blog">部落格</router-link>
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
        justify-content: center;
        gap: 0.5rem;
        padding: 0rem;
        margin: 0rem;
        &>li {
            list-style-type: none;
            &>a {
                display: block;
                padding: 1rem 1rem;
                color: #e0e2e9;
                text-decoration-line: none;
                transition: 200ms;
                &:hover {
                    color: #ffffff;
                    cursor: pointer;
                    background-color: #e0e2e91e;
                }
                // &:is(.router-link-exact-active) {
                //     color: #ffffff;
                //     background-color: #e0e2e91e;
                // }
            }   
        }
    }
}
</style>