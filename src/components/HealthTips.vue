<template>
    <div class="health-tips" id="healthTips">
        <div class="heading">
            <span class="heading-text typography">Health Tips</span>
            <div class="health-tips-arrow-desktop">
                <span class="health-tips-arrow-text typography">Health Tips</span>
                <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
            </div>
        </div>
        <div class="health-tips-div">
            <div class="health-tip">
                <img src="../assets/aproko-doctor.png" alt="aprokoDoctor" class="health-tip-img">
                <div class="health-tip-content">
                    <span class="title">Aproko Doctor</span>
                    <span class="text">Stop smoking Shisha, it kills the Lungs and can shorten life span.</span>
                </div>
            </div>

            <!-- Desktop Template Markup -->

            <div class="health-tip" id="htDesktop">
                <img src="../assets/doctor.png" alt="doctor" class="health-tip-img">
                <div class="health-tip-content">
                    <span class="title">Dr. Olufunmilayo</span>
                    <span class="text">Prevention is absolutely better than cure.</span>
                </div>
            </div>

            <!-- End of Desktop Template Markup -->

            <div class="health-tip">
                <img src="../assets/doctor-anuu.png" alt="doctorAnuu" class="health-tip-img">
                <div class="health-tip-content">
                    <span class="title">Doctor Anuu</span>
                    <span class="text">Eat more protein as your body needs something to build on.</span>
                </div>
            </div>
        </div>
        <div class="health-tips-arrow-mobile">
            <span class="health-tips-arrow-text typography">Health Tips</span>
            <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
        </div>
    </div>
</template>

<script>
export default {
    name: 'HealthTips'
}
</script>

<style scoped>

    /* Desktop Styles */

        @media screen and (min-width: 650px) {

            #healthTips {
                border-top: 0px solid #F6F6F6;
                border-radius: 0;
                box-shadow: 0 0 black;
            }

            .health-tips .health-tips-arrow-mobile {
                display: none;
            }

            .health-tips .heading {
                border-top: 1px solid #D0CDE1;
                border-bottom: 0;
                padding-left: 7%;
                padding-right: 7%;
                display: flex;
                justify-content: space-between;
            }

            .heading .health-tips-arrow-desktop {
                display: flex;
                align-items: center;
                justify-content: space-between;
                width: 21%;
            }

            .health-tips-arrow-desktop .health-tips-arrow-text {                
                color: #2F2E41;
            }

            .health-tips-div .health-tip {
                width: 32%;
            }

            .health-tips-div #htDesktop {
                display: flex;
            }

            .health-tip .health-tip-img {
                border-bottom: 4px solid #46E146;
            }

            #htDesktop .health-tip-content {
                margin-top: 30px;
            }

            .health-tip-content .title {
                color: #0F6D0F;
                font-weight: bold;
            }

        }

    /* End of Desktop Styles */

    .health-tips {
        margin-top: 3rem;
        border-top: 7px solid #2D8CFF;
        border-radius: 16px;
        box-shadow: 0 3px 6px #00000029;
    }

    .health-tips-arrow-desktop, #htDesktop {
        display: none;
    }

    .typography {
        font-family: Georgia, 'Times New Roman', Times, serif;
    }

    .heading {
        border-bottom: 1px solid #95989A;
        padding: 2rem 0;
        margin-bottom: 0.5rem;
        padding-left: 10%;
    }

    .heading-text {
        font-size: 20px;
        color: #333333;
        font-weight: bold;
    }

    .health-tips-div {
        display: flex;
        justify-content: space-between;
        width: 85%;
        margin: auto;
        margin-top: 1.5rem;
    }

    .health-tip {
        display: flex;
        flex-direction: column;
        width: 48%;
    }

    .health-tip-img {
        width: 100%;
        border-radius: 8px;
        box-shadow: 0 3px 6px #00000029;
    }

    .health-tip-content {
        display: flex;
        flex-direction: column;
        margin-top: 20px;
    }

    .title {
        color: #2D8CFF;
        font-size: 12px;
        height: 20%;
        margin-top: 10%;
    }

    .text {
        color: #707070;
        font-size: 14px;
        height: 80%;
        margin-top: 10%;
        line-height: 25px;
    }

    .health-tips-arrow-mobile {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 19%;
        margin-left: 70%;
        padding-bottom: 1.5rem;
        margin-top: 20%;
    }

    .health-tips-arrow-text {
        color: #46E146;
        font-weight: bold;
        font-size: 12px;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .health-tips-arrow-mobile {
                width: 35%;
                margin-left: 55%;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .health-tips-arrow-mobile {
                width: 30%;
                margin-left: 65%;
            }

        }

        @media only screen and (max-width: 550px) and (min-width: 450px) {

            .health-tips-arrow-mobile {
                width: 23%;
            }

        }

        @media only screen and (max-width: 750px) and (min-width: 650px) {

            

        }

        @media only screen and (max-width: 1050px) and (min-width: 850px) {

            

        }

        @media only screen and (max-width: 1150px) and (min-width: 1050px) {

            

        } 

        @media only screen and (min-width: 1150px) {

            #htDesktop .health-tip-img {
                height: 66%;
            }

            #htDesktop .health-tip-content {
                margin-top: 20px;
            }

        }       

    /* End of Responsive Styles */

</style>