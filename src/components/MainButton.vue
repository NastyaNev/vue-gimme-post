<template>
    <button>
        <p>Add Post</p>
    </button>
</template>

<script>
export default {
    name: "main-button",

}
</script>

<style scope>
button {
    position: relative;
    margin: 0;
    padding: 0;
    border: 0;
    border-radius: 16px;
    background: radial-gradient(circle farthest-corner at 100% -25%, white 5%, #92e4e6, #4ca1af 35%);
    padding: 16px 24px;
    border: none;
    color: white;
    cursor: pointer;
    line-height: 0;
    display: flex;
    align-items: center;
    z-index: 150;

    p {
        z-index: 161;
        margin: 0;
        font-weight: bold;
        font-family: 'Montserrat';
    }

    &::before {
        position: absolute;
        content: "";
        inset: 0;
        z-index: 149;
        background: radial-gradient(circle farthest-corner at 0% 0%, white 5%, #92e4e6, #4ca1af 35%);
        opacity: 0;
        transition: opacity 0.25s linear;
        margin: 0;
        padding: 0;
        border: 0;
        border-radius: 16px;
        padding: 16px 24px;
        border: none;
        color: white;
        cursor: pointer;
        line-height: 0;
        display: flex;
        align-items: center;
    }

    &:hover::before {
        opacity: 1;
    }

    &:after {
        content: "";
        background: radial-gradient(circle farthest-corner at 0% 0%, white 5%, #92e4e6, #4ca1af 95%);
        display: block;
        position: absolute;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        opacity: 0;
        transition: all 0.8s;
        z-index: 160;
        border-radius: 16px;
    }

    &:active:after {
        opacity: 1;
        transition: 0s
    }
}
</style>