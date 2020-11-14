<template>
    <div class="meet-the-law" id="meetTheLaw">
        <div class="heading">
            <span class="text">Meet The Law</span>
            <div class="meet-the-law-arrow-desktop">
                <span class="meet-the-law-arrow-text typography">Meet The Law</span>
                <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
            </div>
        </div>
        <div class="card-and-content">
            <div class="card">
                <img src="../assets/barrister-oladimeji.png" alt="barrister" class="card-img">
                <div class="card-text">
                    <span class="title">Bar. Oladimeji Rilwan Esq</span>
                    <span class="body">The Nigerian Constitution as regards Police and Policing</span>
                </div>
            </div>
            <div class="content">
                <span class="content-title typography">The Nigerian Constitution as regards Police and Policing</span>
                <div class="content-item">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">What are my constitutional rights as a Nigerian citizen?</span>
                </div>
                <div class="content-item">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">Understand the 1999 Nigerian constitution</span>
                </div>
                <div class="content-item">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">What are my constitutional rights as a Nigerian</span>
                </div>
                <div class="content-item ci-desktop">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">What are my constitutional rights as a Nigerian citizen?</span>
                </div>
                <div class="content-item ci-desktop">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">Understand the 1999 Nigerian constitution</span>
                </div>
                <div class="content-item ci-desktop">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">What are my constitutional rights as a Nigerian</span>
                </div>
                <div class="content-item ci-desktop">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">Understand the 1999 Nigerian constitution</span>
                </div>
                <div class="content-item ci-desktop">
                    <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                    <span class="content-item-text">What are my constitutional rights as a Nigerian</span>
                </div>
            </div>
        </div>
        <div class="meet-the-law-arrow-mobile">
            <span class="meet-the-law-arrow-text typography">Meet The Law</span>
            <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
        </div>
    </div>
</template>

<script>
export default {
    name: 'MeetTheLaw'
}
</script>

<style scoped>

    /* Desktop Styles */

        @media screen and (min-width: 650px) {

            .meet-the-law .meet-the-law-arrow-mobile, .card .card-text .body {
                display: none;
            }
            
            #meetTheLaw {
                border-top: 0px solid #F6F6F6;
                border-radius: 0;
                box-shadow: 0 0 black;
            }

            .heading .meet-the-law-arrow-desktop {
                display: flex;
                align-items: center;
                justify-content: space-between;
                width: 21%;
            }

            .heading .meet-the-law-arrow-desktop .meet-the-law-arrow-text {
                color: #333333;
            }

            .meet-the-law .heading {
                border-top: 1px solid #D0CDE1;
                border-bottom: 0;
                padding-left: 7%;
                padding-right: 7%;
                display: flex;
                justify-content: space-between;
            }

            .card-and-content {
                display: flex;
                justify-content: space-between;
                width: 90%;
                margin: auto;
            }

            .card-and-content .card {
                margin: 0;
                box-shadow: none;
                width: 49%;
            }

            .card-and-content .content {
                margin: 0;
                background-color: #ffffff;
                padding: 20px;
                width: 49%;
            }

            .card .card-img {
                border-bottom: 6px solid #46E146;
            }

            .card .card-text {
                height: fit-content;
            }

            .card-text .title {
                color: #0F6D0F;
                font-weight: bold;
                margin-top: 1.5rem;
            }

            .content .ci-desktop {
                display: flex;
            }

            .content .content-title {
                display: block;
                color: #333333;
                font-weight: bold;
                font-size: 16px;
                margin-bottom: 1.5rem;
            }

            .content-item .content-item-text {
                font-size: 12px;
            }

        }

    /* End of Desktop Styles */
    
    .meet-the-law {
        border-top: 7px solid #95989A;
        margin-top: 3rem;
        border-radius: 16px;
        box-shadow: 0 3px 6px #00000029;
    }

    .meet-the-law-arrow-desktop, .ci-desktop, .content-title {
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

    .text {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 20px;
        color: #333333;
        font-weight: bold;
    }

    .card {
        width: 85%;
        margin: auto;
        box-shadow: 0 3px 6px #00000012;
        border-radius: 6px;
        margin-top: 1.5rem;
    }

    .card-img {
        width: 100%;
        box-shadow: 0 3px 6px #00000012;
        border-radius: 8px;
    }

    .card-text {
        display: flex;
        flex-direction: column;
        height: 15vh;
        justify-content: space-around;
    }

    .title {
        color: #707070;
        font-size: 12px;
    }

    .body {
        color: #2D8CFF;
        font-weight: bold;
        font-size: 15px;
    }

    .content {
        width: 85%;
        margin: auto;
        margin-top: 1rem;
    }

    .content-item {
        display: flex;
        width: 100%;
        align-items: flex-start;
    }

    .red-pin {
        width: 5%;
    }

    .content-item-text {
        color: #484848;
        width: 75%;
        margin-left: 4%;
        margin-bottom: 1rem;
    }

    .meet-the-law-arrow-mobile {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 28%;
        margin-left: 65%;
        padding-bottom: 1.5rem;
    }

    .meet-the-law-arrow-text {
        color: #46E146;
        font-weight: bold;
        font-size: 12px;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .meet-the-law-arrow-mobile {
                width: 45%;
                margin-left: 50%;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .meet-the-law-arrow-mobile {
                width: 35%;
                margin-left: 55%;
            }

        }

        @media only screen and (max-width: 850px) and (min-width: 650px) {

            .card .card-img[data-v-3b5444c8] {
                border-bottom: 6px solid #46E146;
                height: 60vh;
            }

            .card-and-content .card[data-v-3b5444c8] {
                background-color: #ffffff;
            }

        }

    /* End of Responsive Styles */

</style>