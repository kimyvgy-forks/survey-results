<template>
    <h3 class="entry">
        <a
            v-scroll-to="`#${entry}`"
            :href="`#${entry}`"
            class="h3"
        >
            {{ entry }}
        </a>
    </h3>
</template>

<script>
    export default {
        props: {
            entry: {
                type: String
            }
        }
    }
</script>

<style lang="scss">
    .entry {
        height: 50px;
        width: 100%;
        border-left: 5px solid #5aa1e7;
        display: flex;
        align-items: center;
        background-color: #f6f6f6;
        margin-bottom: 10px;

        a {
            margin-left: 30px;
            text-transform: capitalize;
        }
    }
</style>
