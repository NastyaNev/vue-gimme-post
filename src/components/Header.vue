<template>
    <header>
        <div>
            <img src="../assets/logo.svg" alt="logo" />
            <MainButton />
        </div>
    </header>
</template>

<script>
import MainButton from "./MainButton.vue"
export default {
    name: "app-header",
    components: {
        MainButton
    }
}
</script>

<style scoped>
header {
    box-shadow: 0 0 12px rgba(0, 0, 0, 0.18);
    width: 100vw;
    height: 60px;
    display: flex;
    align-items: center;
    position: fixed;
    z-index: 100;
    justify-content: center;
    background-color: white;

    div {
        width: calc(100vw - 80px);
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;

        img {
            height: 40px;
            transition: opacity 0.3s ease-in-out;
            cursor: pointer;

            &:hover {
                opacity: 0.7;
            }
        }
    }
}
</style>