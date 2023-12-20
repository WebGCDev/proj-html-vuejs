<script>
export default {
    name: "CleanButton",
    props: {
        text: String,
        type: String,
    }
};
</script>

<template>
    <button :class="type === 'secondary' ? 'secondary' : ''" role="button">{{ text }}</button>
</template>

<style scoped>
button {
    border-radius: 5px;
    text-transform: uppercase;
    padding: 10px 20px;
    border: none;
    background-color: #038384;
    color: whitesmoke;
}

.secondary {
    background-color: transparent;
    border: 1px solid #038384;
    padding-left: 20px;
    padding-right: 20px;
}
</style>