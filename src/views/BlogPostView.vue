<template>
    <div class="blog-post">
        <div class="content">
            <h1>{{ message }} Git 使用完全攻略</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores et quisquam iste labore aut repellendus, nobis nisi, aperiam consequuntur, numquam sit consequatur quam nam tempore unde eius optio. Voluptates, accusantium quibusdam nihil exercitationem architecto consequatur excepturi, mollitia error odit delectus incidunt. Dolorem, eaque! Veniam sed exercitationem temporibus dolorem voluptates ab voluptatum nihil soluta quisquam, omnis repellendus eveniet? Minus ab neque, rerum totam ullam quod ipsum. Modi unde nostrum, ipsa odit perspiciatis nisi id quasi, officiis necessitatibus cumque ullam! Quos aliquid consequatur reiciendis similique, maxime distinctio consequuntur asperiores doloremque? Amet ex blanditiis tenetur provident, vitae officia odio temporibus ipsa obcaecati magni.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores et quisquam iste labore aut repellendus, nobis nisi, aperiam consequuntur, numquam sit consequatur quam nam tempore unde eius optio. Voluptates, accusantium quibusdam nihil exercitationem architecto consequatur excepturi, mollitia error odit delectus incidunt. Dolorem, eaque! Veniam sed exercitationem temporibus dolorem voluptates ab voluptatum nihil soluta quisquam, omnis repellendus eveniet? Minus ab neque, rerum totam ullam quod ipsum. Modi unde nostrum, ipsa odit perspiciatis nisi id quasi, officiis necessitatibus cumque ullam! Quos aliquid consequatur reiciendis similique, maxime distinctio consequuntur asperiores doloremque? Amet ex blanditiis tenetur provident, vitae officia odio temporibus ipsa obcaecati magni.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores et quisquam iste labore aut repellendus, nobis nisi, aperiam consequuntur, numquam sit consequatur quam nam tempore unde eius optio. Voluptates, accusantium quibusdam nihil exercitationem architecto consequatur excepturi, mollitia error odit delectus incidunt. Dolorem, eaque! Veniam sed exercitationem temporibus dolorem voluptates ab voluptatum nihil soluta quisquam, omnis repellendus eveniet? Minus ab neque, rerum totam ullam quod ipsum. Modi unde nostrum, ipsa odit perspiciatis nisi id quasi, officiis necessitatibus cumque ullam! Quos aliquid consequatur reiciendis similique, maxime distinctio consequuntur asperiores doloremque? Amet ex blanditiis tenetur provident, vitae officia odio temporibus ipsa obcaecati magni.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores et quisquam iste labore aut repellendus, nobis nisi, aperiam consequuntur, numquam sit consequatur quam nam tempore unde eius optio. Voluptates, accusantium quibusdam nihil exercitationem architecto consequatur excepturi, mollitia error odit delectus incidunt. Dolorem, eaque! Veniam sed exercitationem temporibus dolorem voluptates ab voluptatum nihil soluta quisquam, omnis repellendus eveniet? Minus ab neque, rerum totam ullam quod ipsum. Modi unde nostrum, ipsa odit perspiciatis nisi id quasi, officiis necessitatibus cumque ullam! Quos aliquid consequatur reiciendis similique, maxime distinctio consequuntur asperiores doloremque? Amet ex blanditiis tenetur provident, vitae officia odio temporibus ipsa obcaecati magni.</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores et quisquam iste labore aut repellendus, nobis nisi, aperiam consequuntur, numquam sit consequatur quam nam tempore unde eius optio. Voluptates, accusantium quibusdam nihil exercitationem architecto consequatur excepturi, mollitia error odit delectus incidunt. Dolorem, eaque! Veniam sed exercitationem temporibus dolorem voluptates ab voluptatum nihil soluta quisquam, omnis repellendus eveniet? Minus ab neque, rerum totam ullam quod ipsum. Modi unde nostrum, ipsa odit perspiciatis nisi id quasi, officiis necessitatibus cumque ullam! Quos aliquid consequatur reiciendis similique, maxime distinctio consequuntur asperiores doloremque? Amet ex blanditiis tenetur provident, vitae officia odio temporibus ipsa obcaecati magni.</p>    
        </div>
        <div class="comments">
            <h3>文章留言</h3>
            <CommentCard username="Dada878" message="Lorem ipsum, dolor sit amet consectetur adipisicing elit. Esse vitae et corrupti ipsum, tenetur, consequatur unde dicta eveniet explicabo architecto quod velit natus fuga dolorem iste placeat eius fugit distinctio, quidem eaque molestiae? Veniam dolor, omnis illo quae tempore repellat!" />
            <CommentCard username="Dada878" message="quidem eaque molestiae? Veniam dolor, omnis illo quae tempore repellat!" />
            <div class="new-comment">
                <input type="text">
                <textarea></textarea>
            </div>
        </div>
    </div>
</template>
<script lang="ts" setup>
import CommentCard from '@/components/CommentCard.vue';
import { ref } from 'vue';
import { useRouter } from 'vue-router';
const router = useRouter();
const message = ref("");
message.value = router.currentRoute.value.params.id as string;
</script>
<style lang="scss" scoped>
.blog-post {
    text-align: left;
    margin-left: 20%;
    margin-right: 20%;
    background-color: #364049b0;
    color: #e0e2e9cb;
    font-size: 20px;
    .content {
        padding: 3rem;
        padding-top: 5rem;
        padding-bottom: 0rem;
    }
    .comments {
        padding: 3rem;
        padding-top: 0rem;
        display: flex;
        flex-direction: column;
        gap: 1rem;
        .new-comment {
            padding: 1rem;
            background-color: #47525e;
            border-radius: 1rem;
            display: flex;
            flex-direction: column;
            gap: 1rem;
            input, textarea {
                border-radius: 1rem;
                padding: 1rem;
                background-color: #364049b0;
                border: none;
                outline: none;
                color: rgba(224, 226, 233, 0.7960784314);
            }
        }
        h3 {
            margin-bottom: 0rem;
        }
    }
}
</style>