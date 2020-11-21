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
                margin-right: 1%;
            }

            .heading .meet-the-law-arrow-desktop .meet-the-law-arrow-text {
                color: #333333;
                white-space: nowrap;
                margin-right: 5%;
            }

            .meet-the-law .heading {
                /* border-top: 1px solid #D0CDE1; */
                border-bottom: 0;
                padding-left: 2%;
                padding-right: 2%;
                display: flex;
                justify-content: space-between;
            }

            .card-and-content {
                display: flex;
                justify-content: space-between;
                width: 96%;
                margin: auto;
                height: 350px;
            }

            .card-and-content .card {
                margin: 0;
                box-shadow: none;
                width: 50%;
            }

            .card-and-content .content {
                margin: 0;
                background-color: #ffffff;
                padding: 20px;
                width: 49%;
                box-shadow: 0 3px 6px #00000029;
                border-radius: 5px;
            }

            .card .card-img {
                border-bottom: 6px solid #46E146;
                height: 100%;
            }

            .card .card-text {
                height: fit-content;
            }

            .card-text .title {
                color: #0F6D0F;
                font-weight: bold;
                margin-top: 1%;
                margin-left: 2%;
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
        padding-left: 2%;
    }

    .text {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 30px;
        color: #333333;
        font-weight: bold;
    }

    .card {
        width: 96%;
        margin: auto;
        /* box-shadow: 0 3px 6px #00000012; */
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
        width: 96%;
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
        justify-content: flex-end;
        margin-right: 3%;
        padding-bottom: 1.5rem;
    }

    .meet-the-law-arrow-text {
        color: #46E146;
        font-weight: bold;
        font-size: 12px;
        margin-right: 3%;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            /* .meet-the-law-arrow-mobile {
                width: 45%;
                margin-left: 50%;
            } */

        }

        @media only screen and (max-width: 650px) and (min-width: 300px) {

            .card::after {
                content: "";
                border-bottom: 2px solid #00000012;
                width: 100%;
                left: 0;
                position: absolute;
            }

        }

        @media only screen and (max-width: 850px) and (min-width: 650px) {

            .card .card-img[data-v-3b5444c8] {
                border-bottom: 6px solid #46E146;
            }

            .card-and-content {
                height: 450px;
            }

            .card-and-content .card[data-v-3b5444c8] {
                background-color: #ffffff;
            }

        }

        @media only screen and (min-width: 1000px) {

            .card-and-content {
                height: 500px;
            }

            .card-and-content .content {
                padding-top: 30px;
            }

            .content .content-title {
                font-size: 18px;
            }

            .content-item .content-item-text {
                font-size: 16px;
            }

        }

    /* End of Responsive Styles */

</style>