<script>
import Vehicle from './Vehicle.vue';
import CleanButton from './CleanButton.vue'
import CleanLogo from './CleanLogo.vue';
import SendAMessage from './SendAMessage.vue'
import allinformation from '../allinformation';
import { library } from "@fortawesome/fontawesome-svg-core";
import { FontAwesomeIcon } from "@fortawesome/vue-fontawesome";
import { faPhone, faEnvelope } from "@fortawesome/free-solid-svg-icons";

library.add(faPhone, faEnvelope);
export default {
    name: "CleanMain",
    componets: {
        Vehicle,
        CleanButton,
        FontAwesomeIcon,
        SendAMessage,
        CleanLogo,
    },
    data() {
        return {
            allinformation,
            vechicleTypes: {
                truck1: {
                    img: 'truck-1.png',
                    type: 'Light',
                    weight: 'Max Weigh 1200kg',
                },
                truck2: {
                    img: 'truck-1.png',
                    type: 'Light',
                    weight: 'Max Weigh 1200kg',
                },
                truck3: {
                    img: 'truck-1.png',
                    type: 'Light',
                    weight: 'Max Weigh 1200kg',
                },
            }
        };
    },
}
</script>

<template>
    <div>
        <!-- WHO WE ARE -->
        <section class="who-we-are">
            <div class="container">
                <div class="row">
                    <div class="col-8 title">
                        <h5 class="presentation">WHO WE ARE</h5>
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
                    <div v-for="auto in    vechicleTypes   " class="col-4">
                        <div class="cont-img">
                            <img :src="`../../src/assets/Images/${auto.img}`" alt="truck">
                            <img src="../../src/assets/Images/truck-1.png" alt="">
                        </div>
                        <h5>{{ auto.type }}</h5>
                        <p></p>
                    </div>


                </div>
            </div>
        </section>
        <!-- ROAD TRANSPORT -->
        <section class="sect-road-transport ">


            <div class="cont-road-transport">
                <span class="presentation">ROAD TRANSPORT</span>

                <h2>Main <span>Services</span></h2>
                <div class="subparagraph d-flex align-items-center justify-content-between">
                    <p>
                        With all of this expertise and capability comes an unrivalled commitment to customer
                        service.We
                        will work hard to undersand your needs in order to develop a productive, long-term
                        partnership.
                    </p>
                    <button>see all</button>
                </div>
                <div class=" row-box">
                    <div class="cont-box ">
                        <h4>Technology</h4>
                        <p>We are continually focused on developing technology solutions adapted to our client's needs.</p>
                        <a href="#">→</a>
                    </div>
                    <div class="cont-box ">
                        <h4>Reefer Cargo</h4>
                        <p>Regular and frequent monitoring from the receipt of the loaded container to final destination.
                        </p>
                        <a href="#">→</a>
                    </div>
                    <div class="cont-box">
                        <h4>Dry Cargo</h4>
                        <p>We work with most types of dry cargo, from valuable cargo to the most dangerous requiring care.
                        </p>
                        <a href="#">→</a>
                    </div>
                </div>
            </div>
        </section>
        <!-- HOW IT WORKS IN PRACTICE -->
        <section id="process" class="logistical ">
            <div class="row justify-content-center">
                <div class="cont-practice col-8 text-center">
                    <h5>How it Works in practice</h5>
                    <h1><span>Logistical</span> Procedure</h1>
                    <p>
                        We Work with innovative methodologies to ensure that the entire
                        delivery process is done from start to finish as planned.
                    </p>
                </div>
            </div>
            <div class="cont-timeline row justify-content-center">
                <div class="col-2 cont-elem-timeline">
                    <button>01</button>
                    <h5>Collection of information</h5>
                    <p>Lorem ipsum dolor sit amet consectetur</p>
                </div>
                <div class="col-2 cont-elem-timeline">
                    <button>02</button>
                    <h5>Service Invoice Sending</h5>
                    <p>Lorem ipsum dolor sit amet consectetur</p>
                </div>
                <div class="col-2 cont-elem-timeline">
                    <button>03</button>
                    <h5>Withdrawal of Cargo</h5>
                    <p>Lorem ipsum dolor sit amet consectetur</p>
                </div>
                <div class="col-2 cont-elem-timeline">
                    <button>04</button>
                    <h5>Transport Customer Order</h5>
                    <p>Lorem ipsum dolor sit amet consectetur</p>
                </div>
                <div class="col-2 cont-elem-timeline">
                    <button>05</button>
                    <h5>Successful Delivery</h5>
                    <p>Lorem ipsum dolor sit amet consectetur</p>
                </div>
            </div>
        </section>
        <!-- WHAT ARE WE DOING SECTION -->
        <section id="testimonials" class="results text-white">
            <div class="container">

                <div class="title">
                    <h5>What are we doing</h5>
                    <h1><span>Results</span> in Numbers</h1>
                </div>
                <div class="content-info row pt-5 text-center">
                    <div class="col-3">
                        <h3>128</h3>
                        <p>Certifications</p>
                    </div>
                    <div class="col-3">
                        <h3>230</h3>
                        <p>Employees</p>
                    </div>
                    <div class="col-3">
                        <h3>517</h3>
                        <p>Customers</p>
                    </div>
                    <div class="col-3">
                        <h3>94</h3>
                        <p>Countries Served</p>
                    </div>
                </div>

            </div>
        </section>
        <!-- CUSTOMERS TESTIMONIALS -->
        <section class="feedback  text-white">
            <div class="container ">
                <div class="row justify-content-center">
                    <div class="col-8 text-center">
                        <h5>Customer testimonials</h5>
                        <h1>Trusted <span>Feedback</span></h1>
                        <p>
                            We Work intensively in search of ideals that can add up in the
                            lives of our curstomers. This is what moves us and we are grateful
                            for the recognition.
                        </p>
                    </div>
                </div>
                <div class="row justify-content-center">
                    <div class="col p-2 feedback-card">
                        <img src="../../src/assets/Images/logo-1.png" alt="WooCommerce" />
                        <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan
                            orci rhoncus at pellentesque.
                            Lorem ipsum solor sit amet, consectetur adipiscing elit
                        </p>
                        <span>"</span>
                    </div>
                    <div class="col mx-3 p-2 feedback-card">
                        <img src="../../src/assets/Images/logo-2.png" alt="WordPress" />
                        <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan
                            orci rhoncus at pellentesque.
                            Lorem ipsum solor sit amet, consectetur adipiscing elit</p>
                        <span>"</span>
                    </div>
                    <div class="col p-2 feedback-card">
                        <img src="../../src/assets/Images/logo-3.png" alt="Pingdom" />
                        <p>Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan
                            orci rhoncus at pellentesque.
                            Lorem ipsum solor sit amet, consectetur adipiscing elit</p>
                        <span>"</span>
                    </div>
                </div>
            </div>
        </section>
        <!-- SEND A MESSAGE CONTACT -->
        <section class="send-message">
            <div class="container pt-5">
                <div class="row">
                    <div class="col-7 my-5">
                        <h5 class="presentation">SEND A MESSAGE</h5>
                        <h1 class="py-3">Get in <span>Touch</span></h1>
                        <p class="py-3">We will respond to your message as soon as possible.</p>

                        <form role="form">
                            <div class="controls">
                                <div class="row">
                                    <div class="col-md-6">
                                        <div class="form-group">
                                            <input type="text" name="name" class="form-control" placeholder="Name" />
                                        </div>
                                    </div>
                                    <div class="col-md-6">
                                        <div class="form-group">
                                            <input type="text" name="email" class="form-control" placeholder="Email" />
                                        </div>
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-md-6 py-3">
                                        <div class="form-group">
                                            <input type="phone" name="phone" class="form-control" placeholder="Phone" />
                                        </div>
                                    </div>
                                    <div class="col-md-6 py-3">
                                        <div class="form-group">
                                            <select id="form_need" name="need" class="form-control">
                                                <option selected disabled value="">More Info <strong
                                                        class="text-end"></strong></option>
                                                <option>Request Invoice for order</option>
                                                <option>Request order status</option>
                                                <option>Haven't received cashback yet</option>
                                                <option>Other</option>
                                            </select>
                                        </div>
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-md-12">
                                        <div class="form-group">
                                            <textarea class="form-control" placeholder="Message" rows="4"></textarea>
                                        </div>
                                    </div>
                                    <div class="col-md-12 py-3">
                                        <input type="submit" class="btn btn-success btn-send pt-2 btn-block" value="Send" />
                                    </div>
                                </div>
                            </div>
                        </form>
                    </div>
                    <div class="example col-5">
                        <ul>
                            <li>
                                <h4>Example Inc.</h4>
                            </li>
                            <li class="py-2">
                                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit</p>
                            </li>
                            <li class="py-1">
                                <p>Praesent diam lacus, dapibus sed imperdiet consectetur</p>
                            </li>
                            <li class="py-3">

                                <span>+ 1 (305 1234-5678)</span>
                            </li>
                            <li class="py-3">

                                <span>hello@example.com</span>
                            </li>
                            <li class="py-3">

                                <span>Main Avenue, 987</span>
                            </li>
                            <li>
                                <button>VIEW MAP</button>
                            </li>
                        </ul>

                    </div>
                </div>
            </div>
        </section>
        <!-- NEXGEN ABOUT-TRANSPORT-SUPPORT -->
        <section class="footer bg-dark py-5 text-white">
            <div class="container">
                <div class="">
                    <div class="col-3">
                        <ul>
                            <li>
                                <CleanLogo />
                            </li>
                            <li>A Functional HTML Template for Corporate & Business.</li>
                            <li>{{ phone }}</li>
                            <li>{{ mail }}</li>
                            <li>{{ street }}</li>
                            <li>
                                <CleanButton />
                            </li>
                        </ul>
                    </div>
                    <div class="col-3">About >The Company >Institutional >Social & Events >Innovation >Environment
                        >Technology
                    </div>
                    <div class="col-3">Transport >Industrialized >Chemicals >Packaged >Liquids >Construction >Laminated Wook
                        >And
                        others</div>
                    <div class="col-3">Responsibility >Terms of Use >About Cookies >Privacy Policy >Accessibility
                        >Information
                    </div>
                </div>
            </div>
        </section>
        <!-- CREDITS FINAL -->
        <section>
            <div id="fixed_footer">
                <div class="container">
                    <div id="credits">
                        <p class="grey">Enjoy the low price. We are tracking any intention of piracy</p>
                        <p class="grey"><i class="far fa-copyright"></i>2020 NEXGEN is Proudly powered by <span
                                class="green">Coding</span></p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<style lang="scss" scoped>
.who-we-are {
    padding-top: 100px;
    padding-bottom: 100px;
}

.important-text {
    border-left: 4px solid rgb(96, 157, 159, 0.4);
    padding-left: 20px;
    font-style: italic;
    color: grey;
}


// WHAT ARE WE DOING SECTION 
.results {
    background-image: url("/src/assets/Images/bg-10.jpg");
    background-size: cover;
    background-position-y: center;
    padding-top: 80px;
    padding-bottom: 200px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .container {
        width: 80%;
        margin: 0 auto;

        .title {

            h5 {
                color: #00A6A6;
                text-transform: uppercase;
                text-align: center;
            }

            h1 {
                text-align: center;
                font-weight: 800;
                margin-top: 30px;

                span {
                    background-color: rgba($color: #214850, $alpha: 0.5);
                    padding: 10px 20px;
                    border-radius: 5px;

                }
            }
        }

        .content-info {
            h3 {
                color: #00A6A6;
                font-size: 40px;
                font-weight: 700;
            }

            p {
                font-weight: 600;
                font-size: 30px;
            }
        }
    }

}



.title ul {
    list-style: disc;
}

.phone {
    background-color: aqua;
    border-radius: 50%;
}

.mail {
    background-color: aqua;
    border-radius: 50%;
}

.street {
    background-color: aqua;
    border-radius: 50%;
}

.form-color {
    background-color: #ececec;
}

// Road Transport
.sect-road-transport {
    background-color: #111117;
    color: #b6c3bf;

    .presentation {
        color: #52bbbb;
        font-size: 14px;
        font-weight: 600;

    }

    h2 {
        color: white;
        font-weight: 800;
        margin: 20px 0;

        span {
            background-color: #0e272d;
            padding: 5px 15px;
            border-radius: 5px;
        }
    }

    .cont-road-transport {
        width: 50%;
        margin: 0 auto;
        padding: 100px 0;

        .subparagraph {
            margin-bottom: 20px;

            p {
                width: 80%;
            }

            button {
                text-transform: uppercase;
                background-color: transparent;
                color: white;
                border: 1px solid #058283;
                padding: 10px 25px;
                border-radius: 8px;
            }
        }

        .row-box {
            display: flex;
            justify-content: space-between;
            gap: 20px;

            .cont-box {
                background-color: #19191f;
                border-radius: 10px;
                padding: 40px;
                position: relative;


                h4 {
                    font-size: 24px;
                    color: white;
                    margin-bottom: 20px;
                }

                a {
                    color: #0f4e51;
                    font-size: 40px;
                    text-decoration: none;
                    position: absolute;
                    top: 0;
                    right: 20px;
                }
            }
        }

    }
}

// PRACTICE

.logistical {
    padding: 100px 0;
    background-color: #EEF4ED;

    .cont-practice {
        h5 {
            text-transform: uppercase;
            font-size: 14px;
            color: #3EABAB;
            padding: 10px;
            font-weight: 600;
        }

        h1 {
            font-weight: 800;
            margin-top: 20px;

            span {
                background-color: #CCE3DE;
                padding: 5px 10px;
                color: #058283;
                border-radius: 5px;
            }
        }

        p {
            font-size: 15px;
            color: rgb(107, 107, 107);
            margin-top: 20px;
        }
    }

    .cont-timeline {
        text-align: center;
        border-top: 5px solid #CCE3DE;
        position: relative;
        margin-top: 50px;


        button {
            color: #058283;
            border-radius: 50%;
            padding: 10px;
            background-color: #DAECED;
            border: none;
            font-weight: 800;
            position: absolute;
            top: -25px;

        }

        h5 {
            margin-top: 50px;
            font-size: 28px;
            font-weight: 700;
            width: 80%;
            margin: 50px auto 20px;
        }

        p {
            width: 80%;
            margin: 0 auto;
        }



    }
}

// CUSTOMERS TESTIMONIALS


.feedback {
    background-color: #111117;
    padding: 150px 0;

    img {
        filter: brightness(0) invert(1);
    }

    h5 {
        color: #00A698;
        text-transform: uppercase;
        font-size: 14px;
    }

    h1 {
        font-size: 60px;
        font-weight: 800;
        padding: 20px 0;

        span {
            background-color: rgba($color: #1b4752, $alpha: 0.5);
            padding: 5px 20px;
            border-radius: 10px;
        }
    }

    p {
        color: rgb(161, 161, 161);
        padding-bottom: 20px;
    }

    .feedback-card {
        background-color: #19191F;
        width: calc(90% / 3);
        border-radius: 15px;
        position: relative;


        img {
            margin: 20px 0 20px 30px;
        }

        p {
            color: rgb(161, 161, 161);
            width: 80%;
            margin: 0 auto;
        }

        span {
            font-size: 50px;
            color: #47474C;
            position: absolute;
            bottom: 0px;
            right: 20px;
        }

    }
}

// SEND A MESSAGE

input {
    background-color: #ececec;
}

option {
    background-color: #ececec;
}

textarea {
    background-color: #ececec;
}

.send-message {
    h5 {
        color: #00A6A6;
    }

    h1 {
        font-size: 50px;
        font-weight: 800;

        span {
            background-color: #DAECED;
            color: #058283;
            padding: 5px 15px;
            border-radius: 10px;
        }
    }
}

.example {
    li {

        p {
            font-size: 22px;
            color: grey;
        }

        span {
            color: #058283;
            font-size: 22px;

        }

        button {
            background-color: transparent;
            border: 1px solid #058283;
            padding: 10px 20px;
            color: #058283;
            border-radius: 5px;
        }
    }
}

//CREDITS FINAL

#credits {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 10px;
    color: #c0c3d0;
}

#fixed_footer p {
    font-size: .7rem;
}

#fixed_footer {
    display: flex;
    justify-content: center;
    max-height: 80px;
    padding: 10px 0;
    background-color: black;
}
</style>