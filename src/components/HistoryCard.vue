<template>
    <section>
        <h1>個人經歷</h1>
        <div class="step">
            <div class="stepper">
                <div class="circle"></div>
                <div class="line"></div>
            </div>
            <div class="content">
                <p>國中</p>
                <p>- 全國貓咪盃 Scratch 競賽遊戲組冠軍</p>
            </div>
        </div>
        <div class="step">
            <div class="stepper">
                <div class="circle"></div>
                <div class="line"></div>
            </div>
            <div class="content">
                <p>高中</p>
                <p>- APCS 實作題達到 4 級分</p>
                <p>- 虎尾 Python 程式設計競賽第 10 名</p>
                <p>- SCIST 資言資語寒訓模擬賽 8 名</p>
                <p>- 銘傳大學 APCS 冬令營金獎第 1 名</p>
                <p>- Codeforces Rating 達到 1200+</p>
                <p>- CPE 檢定達到專家級</p>
            </div>
        </div>
    </section>
</template>
<style lang="scss" scoped>


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