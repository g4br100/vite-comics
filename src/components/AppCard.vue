<script>
export default {
    name: "AppCard",
    props: {
        details: Object,
        linkImg: String,
        nameImg: String
    }
}
</script>

<template>
    <div class="comic">
        <div class="imgcomic">
            <img :src="linkImg" :alt="nameImg">
        </div>
        <h4>{{ nameImg }}</h4>
    </div>
</template>


<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.comic {
    width: calc(100% / 6);
    padding: 10px;
    cursor: pointer;
    text-align: left;

    &:hover {
        filter: brightness(120%);
        color: $primary-color;
        outline: auto;
    }

    .imgcomic {
        height: 180px;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }

    h4 {
        font-size: 12px;
        margin: 10px 0 20px 0;
        text-transform: uppercase;
    }
}
</style>