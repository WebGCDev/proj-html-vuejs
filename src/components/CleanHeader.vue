<script>
import CleanButton from './CleanButton.vue';
import allinformation from '../allinformation'
import CleanLogo from './CleanLogo.vue'
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";

import {
    faPhone,
    faEnvelope,
    faClock,

} from "@fortawesome/free-solid-svg-icons";
import {
    faUser,
} from "@fortawesome/free-regular-svg-icons";
import {
    faFacebookF,
    faTwitter,
    faLinkedinIn,
} from "@fortawesome/free-brands-svg-icons";
library.add(faPhone, faEnvelope, faUser);
library.add(faFacebookF, faTwitter, faLinkedinIn);
library.add(faClock);

export default {
    name: "CleanHeader",
    components: { CleanButton, FontAwesomeIcon, CleanLogo },
    data() {
        return { ...allinformation };
    },
};
</script>

<template>
    <div>
        <div class="text-white navbar">
            <div class="container d-flex justify-content-between align-items-center py-2">
                <div class="d-flex justify-content-evenly align-items-center w-25">
                    <font-awesome-icon class="clock" icon="fa-solid fa-clock" />
                    <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
                </div>
                <div class="d-flex justify-content-evenly align-items-center w-50">
                    <div>
                        <font-awesome-icon class="px-2" icon="fa-solid fa-phone" />
                        <span>{{ phone }}</span>
                    </div>
                    <div>
                        <font-awesome-icon class="px-2" icon="fa-solid fa-envelope" />
                        <span>{{ mail }}</span>
                    </div>
                    <font-awesome-icon icon="fa-brands fa-facebook-f" />
                    <font-awesome-icon icon="fa-brands fa-twitter" />
                    <font-awesome-icon icon="fa-brands fa-linkedin-in" />
                </div>
            </div>
        </div>
        <div class="jumbotron">
            <div class="links container d-flex">
                <ul class="w-25 p-0">
                    <li class="p-0">
                        <CleanLogo />
                    </li>
                </ul>
                <ul class="d-flex align-items-center justify-content-end w-75">
                    <!-- Ti riporta direttamente alla Home con refresh -->
                    <li><a href="">HOME</a></li>
                    <!-- Link che non hanno una pagina di destinazione -->
                    <li class="px-4"><a href="#about">ABOUT</a></li>
                    <li class="px-4"><a href="#services">SERVICES</a></li>
                    <li class="px-4"><a href="#process">PROCESS</a></li>
                    <li class="px-4"><a href="#testimonials">TESTIMONIALS</a></li>
                    <li><font-awesome-icon class="user px-2" icon="fa-regular fa-user" /></li>
                    <li>
                        <CleanButton text="GET IN TOUCH" />
                    </li>
                </ul>
            </div>
            <div class="container jumbotron-description">
                <div class="row">
                    <div class="col-6">
                        <h4 class="paragraph-title">LOGISTICS SERVICES</h4>
                        <h1 class="subtitle text-white">CARGO TRANSPORT</h1>
                        <p class="description">
                            Fractional or exclusive road cargo transportation to all regions,
                            with small, medium and large vehicles.
                        </p>
                        <div class="buttons-container">
                            <CleanButton class="button-primary" text="GET IN TOUCH" />
                            <CleanButton type="secondary" text="READ MORE" />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.jumbotron {
    background-image: url("/src/assets/Images/bg-9.jpg");
    background-size: cover;
    box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.6);

    & .logo {
        width: 150px;
    }

    & ul {
        list-style: none;

        & li {
            padding-left: 0.5rem;
            padding-right: 0.5rem;

            & a {
                text-decoration: none;
                text-transform: uppercase;
                color: white;
            }
        }
    }
}

.user {
    color: white;
}

.subtitle {
    font-size: 5rem;
    text-transform: uppercase;
}

.jumbotron-description {
    padding-top: 7rem;
    padding-bottom: 10rem;

    & .paragraph-title {
        color: #038384;
        text-transform: uppercase;
    }
}

.description {
    font-size: 1.5rem;
    color: grey;
}

.button-primary {
    margin-right: 20px;
}

.navbar {
    background-color: #21333e;
}
</style>
