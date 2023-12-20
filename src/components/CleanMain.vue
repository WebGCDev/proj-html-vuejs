<script>
import Vehicle from './Vehicle.vue';
export default {
    name: "CleanMain",
    componets: {
        Vehicle,
    },
};
</script>

<template>
    <section class="who-we-are">
        <div class="container">
            <div class="row">
                <div class="col-8 title">
                    <h5>WHO WE ARE</h5>
                    <h1>Excellence in Transport</h1>
                    <p class="py-2 text-secondary">
                        The framework used in the Excellence Programme has been developed by the sector, for the sector.
                        Application of this framework highlights the relationships between the drivers of performance
                        and the desired results, with a strong focus on community outcomes and the delivery of benefits.
                    </p>
                    <p class="py-3 text-secondary">
                        The Excellence Programme supports longer term investment confidence and will support an
                        organisation to meet Local Government, Waka Kotahi NZ Transport Agency, ISO standards and IIMM
                        requirements.
                    </p>
                    <p class="py-3 important-text">
                        This framework will help an organisation enable a step change in transport sector capability,
                        provide leadership in improvement of transport outcomes, and shift the culture of transport
                        investment to proactively address future challenges and improve decision making around wellbeing
                        outcomes.
                    </p>
                    <p class="py-3 text-secondary">
                        The Excellence Programme helps organisations identify potential problems and undertake necessary
                        improvements to get back on track.
                    </p>
                    <ul class="text-secondary">
                        <li>Lorem ipsum dolor sit amet</li>
                        <li>Lorem ipsum dolor sit amet</li>
                        <li>Lorem ipsum dolor sit amet</li>
                        <li>Lorem ipsum dolor sit amet</li>
                        <li>Lorem ipsum dolor sit amet</li>
                    </ul>
                </div>
                <div class="col-4">
                    <h5>Vehicle Types</h5>
                    <VehicleTypes />
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss">
.who-we-are {
    padding-top: 100px;
}

.important-text {
    border-left: 4px solid rgb(96, 157, 159, 0.4);
    padding-left: 20px;
    font-style: italic;
    color: grey;
}
</style>