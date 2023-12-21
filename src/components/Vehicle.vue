<script>
export default {
    name: "Vehicle",
    components: {},
    data() {
        return {

        };
    },
};
</script>

<template>
    <div>
        <div class="border-bottom pt-2" v-for="(vehicle, index) in vehicleTypes" :key="index">
            {{ vehicle.type }}
        </div>

        <div class="mt-4">
            <h5>Certifications</h5>
            <figure>
                <img v-for="n in 2" :key="n" class="certificate me-4" src="../assets/Images/certificate.png"
                    alt="Certificate" />
            </figure>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.truck-image {
    width: 100%;
    background-color: #c5f1f3;
    padding: 5px;
}

.vehicle-type {
    font-weight: bold;
    font-size: 1.3rem;
}

.weight {
    color: grey;
}

.certificate {
    width: 110px;
    height: 110px;
}
</style>