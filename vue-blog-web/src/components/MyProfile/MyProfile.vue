<template>
    <div class="my-profile-container">
        <div class="avatar">
            <el-image
                :src="profileUrl"
            />
        </div>
        <p class="name">{{ myIntro.nick_name }}</p>
        <p class="position">{{ myIntro.user_profession }}</p>
        <p class="info">{{ myIntro.user_intro }}</p>
    </div>
</template>

<script>
export default {
    name: "MyProfile",
    props: {
        myIntro: {
            type: Object,
            default: () => {
                return {}
            }
        },
        profileUrl: {
            type: String,
            default: ''
        },


    },
    components: {},
    data() {
        return {}
    },
    methods: {},
    computed: {},
    watch: {},
    mounted() {
    }
}
</script>

<style scoped lang="scss">
@import "MyProfile";
</style>
