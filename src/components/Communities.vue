<template>
    <div class="communities" id="communities">
        <div class="communities-label">
            <span class="label-title communities-typography">Communities</span>
            <div class="communities-label-arrow-desktop">
                <span class="label-arrow-text communities-typography">Communities</span>
                <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
            </div>
        </div>
        <!-- <hr class="communities-body-hr"> -->
        <div class="communities-body">
            <div class="community">
                <div class="community-img">
                    <img src="../assets/communities-1.png" alt="communities1">
                </div>
                <div class="community-text-div">
                    <span class="community-text-title">Tech & Innovations</span>
                    <span class="community-text communities-typography">Pulling a Paystack stunt like a boss!</span>
                </div>
                <div class="community-pinned-text-div">
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">Starting your own Paystack ?</span>
                    </div>
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">Imposter syndromes and how best to knock it out</span>
                    </div>
                </div>
            </div>
            <div class="community">
                <div class="community-img">
                    <img src="../assets/endsars-logo.png" alt="communities2">
                </div>
                <div class="community-text-div">
                    <span class="community-text-title">Youths development</span>
                    <span class="community-text communities-typography">We must ensure youth inclusive governance come 2023: Soyinka.</span>
                </div>
                <div class="community-pinned-text-div">
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">INEC to encourage voters</span>
                    </div>
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">Nigeria is ready for e-voting</span>
                    </div>
                </div>
            </div>
            <div class="community last-community">
                <div class="community-img">
                    <img src="../assets/communities-3.png" alt="communities3">
                </div>
                <div class="community-text-div">
                    <span class="community-text-title">Politics</span>
                    <span class="community-text communities-typography">International communities stands with peaceful protesters.</span>
                </div>
                <div class="community-pinned-text-div">
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">Nigerians in diaspora are actively protesting</span>
                    </div>
                    <div class="content-item">
                        <img src="../assets/red-pin.svg" alt="redPin" class="red-pin">
                        <span class="content-item-text">Lewis Hamilton supports End Sars peaceful protesters</span>
                    </div>
                </div>
            </div>
        </div>
        <div class="communities-label-arrow-mobile">
            <span class="label-arrow-text communities-typography">Communities</span>
            <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Communities'
}
</script>

<style scoped>

    /* Desktop Styles */

        @media screen and (min-width: 650px) {

            #communities {
                border-top: 0px solid #F6F6F6;
                border-radius: 0;
                box-shadow: 0 0 black;
                margin-top: 0;
            }

            .communities .communities-label-arrow-mobile {
                display: none;
            }

            .communities .communities-label-arrow-desktop {
                display: flex;
                align-items: center;
                margin-right: 1%;
                /* justify-content: space-between;
                width: 21%; */
            }

            .communities .communities-label-arrow-desktop .label-arrow-text {
                color: #333333;
                margin-right: 5%;
            }

            .communities .communities-label {
                border-bottom: 0;
                padding-left: 3%;
                padding-right: 3%;
                justify-content: space-between;
            }

            .communities .communities-body-hr {
                display: block;
                border-top: 1px solid #D0CDE1;
                width: 96%;
                position: absolute;
                top: 0;
                left: 2%;
            }

            .communities .communities-body {
                flex-direction: row;
                width: 97%;
                margin: auto;
            }

            .communities-body .community {
                /* border-bottom: 0; */
                flex-direction: column;
                width: 32%;
                /* padding-bottom: 0; */
                justify-content: space-around;
                margin: 0 auto;
            }

            .communities-body .last-community {
                margin-bottom: 0;
                margin-top: 1%;
                border-bottom: 1px solid #00000029;
            }

            .community:first-child .community-text-div .community-text-title {
                margin-top: 5%;
            }

            .last-community .community-text-div .community-text-title {
                margin-top: 9%;
            }

            .community .community-img {
                width: 100%;
            }

            .community .community-text-div {
                width: 100%;
                margin-left: 0;
            }

            .community-text-div .community-text-title {                
                margin-left: 5%;
                margin-top: 1%;
            }

            .community-text-div .community-text {
                margin-top: 3%;
                height: 60px;
                margin-left: 5%;
            }

            .community .community-img img {
                border-bottom: 5px solid #46E146;
            }

            .community .community-pinned-text-div {
                display: flex;
                flex-direction: column;
                width: 95%;
                margin-left: 5%;
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
                color: #0F6D0F;
                width: 75%;
                margin-left: 4%;
                margin-bottom: 1rem;
                font-size: 11px;
            }

        }

    /* End of Desktop Styles */

    .communities-typography {
        font-family: Georgia, 'Times New Roman', Times, serif;
    }

    .communities {
        border-top: 7px solid #F9EA11;
        margin-top: 3rem;
        border-radius: 16px;
        box-shadow: 0 3px 6px #00000029;
        position: relative;
    }

    .communities-label {
        display: flex;
        border-bottom: 1px solid #D0CDE1;
        padding: 2rem 0;
        margin-bottom: 1.5rem;
        padding-left: 2%;
    }

    .communities-label-arrow-desktop, .community-pinned-text-div, .communities-body-hr {
        display: none;
    }

    .communities-label-arrow-mobile {
        display: flex;
        align-items: center;
        justify-content: flex-end;
        padding-bottom: 1.5rem;
    }

    .label-title {
        color: #333333;
        font-weight: bold;
        font-size: 30px;
    }

    .label-arrow-text {
        color: #46E146;
        font-weight: bold;
        font-size: 12px;
        margin-right: 2%;
    }

    .right-arrow {
        margin-right: 3%;
    }

    .communities-body {
        display: flex;
        flex-direction: column;
    }

    .community {
        display: flex;
        justify-content: space-between;
        width: 96%;
        margin: auto;
        border-bottom: 1px solid #00000029;
        margin-bottom: 1.5rem;
        padding-bottom: 10px;
    }

    .last-community {
        border-bottom: 0px;
        margin-bottom: 1rem;
    }

    .community-img {
        width: 50%;
    }

    .community-img img {
        width: 100%;
        height: 100%;
        border-radius: 16px;
    }

    .community-text-div {
        display: flex;
        flex-direction: column;
        width: 50%;
        margin-left: 5%;
        justify-content: space-evenly;
    }

    .community-text-title {
        /* font-style: italic; */
        font-size: 12px;
        color: #0F6D0F;
        font-weight: 600;
    }

    .community-text {
        color: #333333;
        font-size: 16px;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .communities-label-arrow-mobile {
                width: 45%;
                margin-left: 50%;
            }
    
        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .communities-label-arrow-mobile {
                width: 35%;
                margin-left: 60%;
            }

        }

        @media only screen and (max-width: 550px) and (min-width: 450px) {

            

        }

        @media only screen and (max-width: 750px) and (min-width: 650px) {

            

        }

        @media only screen and (max-width: 1050px) and (min-width: 850px) {

            

        }

        @media only screen and (max-width: 1150px) and (min-width: 1050px) {

            

        } 

        @media only screen and (min-width: 1050px) {

            .communities-body .last-community {
                margin-top: 0;
            }

            .community:first-child .community-text-div .community-text-title {
                margin-top: 0;
            }

            .last-community .community-text-div .community-text-title {
                margin-top: 2%;
            }

        }       

    /* End of Responsive Styles */

</style>
