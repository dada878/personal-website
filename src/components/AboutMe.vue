<template>
    <div class="aboutme">
        <section class="histroy">
            <h1>個人學/經歷</h1>
            <div class="step">
                <div class="stepper">
                    <div class="circle"></div>
                    <div class="line"></div>
                </div>
                <div class="content">
                    <p>育林國小</p>
                    <p>- 入門 HTML、Python</p>
                    <p>- 熟練 Scratch</p>
                </div>
            </div>
            <div class="step">
                <div class="stepper">
                    <div class="circle"></div>
                    <div class="line"></div>
                </div>
                <div class="content">
                    <p>福豐國中</p>
                    <p>- 全國貓咪盃 Scartch 競賽遊戲組冠軍</p>
                    <p>- 網頁前端入門 Javascript、CSS</p>
                    <p>- 網頁後端入門 SQL、PHP</p>
                    <p>- APP開發入門 Flutter、Dart</p>
                    <p>- 遊戲開發入門 Unity、C#</p>
                </div>
            </div>
            <div class="step">
                <div class="stepper">
                    <div class="circle"></div>
                    <div class="line"></div>
                </div>
                <div class="content">
                    <p>振聲高中</p>
                    <p>- C++ 入門</p>
                    <p>- 競賽程式入門</p>
                    <p>- APCS 實作題達到 4 級分</p>
                    <p>- 虎尾科大 Python 程式設計競賽決賽第 10 名</p>
                    <p>- 銘傳大學 APCS 冬令營金獎第 1 名</p>
                </div>
            </div>
        </section>
        <section class="about">
            <h1>關於</h1>
            <p>我是一個剛入坑競程的高中生</p>
            <p>實作領域較擅長網頁前端開發與 Python 實作專案</p>
            <p>目標是可以透過特殊選材上不錯的大學</p>
            <p>這是使用 Vue.js 框架建立的網站</p>
            <p>希望未來可以繼續累積更多作品與文章在這裡</p>
        </section>
        <section class="skills">
            <h1>技能</h1>
            <div class="skillcards">
                <div>
                    <font-awesome-icon icon="fa-brands fa-python" />
                    <h3>Python 3 年</h3>
                    <button>查看相關作品</button>
                </div>
                <div>
                    <font-awesome-icon icon="fa-brands fa-html5" />
                    <h3>網頁前端開發 3 年</h3>
                    <button>查看相關作品</button>
                </div>
                <div>
                    <font-awesome-icon icon="fa-brands fa-unity" />
                    <h3>Unity 遊戲開發 1 年</h3>
                    <button>查看相關作品</button>
                </div>
            </div>

        </section>
    </div>
</template>
  
<script lang="ts" setup>

</script>
  
<style scoped lang="scss">
.about {
    padding-bottom: 2rem;
}

.skills {
    .skillcards {
        display: flex;
        padding-left: 1rem;
        padding-right: 1rem;
        padding-bottom: 1rem;
        align-items: stretch;
        gap: 1rem;

        h3 {
            margin: 0rem;
        }

        div {
            flex: 1;
            background-color: #47525e;
            border-radius: 1rem;
            padding: 1rem;
            padding-top: 2rem;
            height: 100%;

            button {
                background-color: #626d79;
                border-radius: 0.3rem;
                border: none;
                padding: 0.5rem;
                margin-top: 1rem;
                width: 100%;
                color: inherit;
                transition: 200ms;

                &:hover {
                    background-color: #6f7a86;
                    cursor: pointer;
                }
            }

            svg {
                font-size: 5rem;
                margin-bottom: 1rem;
            }
        }
    }
}

.aboutme {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(4, 1fr);
    grid-column-gap: 1rem;
    grid-row-gap: 1rem;
    padding-top: 2rem;
    padding-bottom: 2rem;
    padding-left: 7rem;
    padding-right: 7rem;

    &>* {
        background-color: #364049;
        border-radius: 1rem;
        padding-left: 1rem;
        padding-right: 1rem;
        overflow: hidden;

        &>h1 {
            font-weight: 400;
            font-size: calc(1rem + 1vw);
        }
    }

    .histroy {
        grid-area: 1 / 1 / 5 / 3;
    }

    .about {
        grid-area: 1 / 3 / 3 / 6;
    }

    .skills {
        grid-area: 3 / 3 / 5 / 6;
    }
}

.step {
    padding: 10px;
    display: flex;
    flex-direction: row;
    gap: 1rem;
    justify-content: flex-start;

    .stepper {
        position: relative;

        .circle {
            background-color: rgb(209, 209, 209);
            border: 3px solid gray;
            border-radius: 100%;
            width: 20px;
            height: 20px;
            display: inline-block;
            visibility: visible;
            border-color: rgb(140, 143, 145)
        }

        .line {
            top: 23px;
            left: 12px;
            height: 100%;
            position: absolute;
            border-left: 3px solid gray;
            border-left: 3px solid rgb(140, 143, 145);
        }
    }

    .content {
        padding-top: 3px;

        p {
            text-align: left;
            margin-top: 1rem;
            margin-bottom: 0rem;

            &:nth-child(1) {
                font-weight: bold;
                margin: 0rem;
            }
        }
    }
}
</style>
  