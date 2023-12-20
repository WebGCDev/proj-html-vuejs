<script>
export default {
    name: "Vehicle",
    props: { text: String, type: String },
    data() {
        return {
        }
    },
};
</script>

<template>
    <div>
        <img :src="require('@/assets/Images/truck-1.png')" alt="TruckTypes" />
        <p>Lorem ipsum dolor sit amet
        </p>
    </div>
</template>

<style lang="scss" scoped></style>