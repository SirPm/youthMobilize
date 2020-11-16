<template>
    <div class="below-header">
        <img src="../assets/caution-img.svg" alt="caution-img" class="caution-img">
        <div class="below-header-div">
            <div class="end-sars-div">
                <span class="end-sars below-header-gen">End Sars</span>
            </div>
            <div class="aisha">
                <img src="../assets/aisha.png" alt="aisha">
            </div>
            <div class="it">
                <div class="rcc">
                    <span class="rcc-text below-header-gen">Report</span>
                    <span class="rcc-text below-header-gen">Challenge</span>
                    <span class="rcc-text below-header-gen">Change</span>
                </div>
                <div class="it-text-div">
                    <span class="it-text below-header-gen">It</span>
                </div>
            </div>
        </div>
        <img src="../assets/caution-img.svg" alt="caution-img" class="caution-img">
    </div>
</template>

<script>
export default {
    name: 'BelowHeader'
}
</script>

<style scoped>

    @media screen and (min-width: 650px) {

        .below-header {
            display: flex;
            width: 90%;
            margin: auto;
        }

        .below-header .caution-img {
            display: block;
            width: 8%;
        }

        .below-header .below-header-div {
            width: 80%;
            margin: 2rem auto;
            border-radius: 10px;
        }

        .below-header .below-header-div .it {
            border-top-right-radius: 10px;
            border-bottom-right-radius: 10px;
        }

        .end-sars-div .end-sars {
            font-size: 2.9rem;
        }

        .it-text-div .it-text {
            font-size: 120px;
        }
    }

    .below-header-gen {
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: bold;
    }

    .caution-img {
        display: none;
    }

    .below-header-div {
        display: flex;
        box-shadow: 0 3px 6px #B7A71B;
        margin-top: 2rem;
    }

    .end-sars-div {
        display: flex;
        width: 25%;
        align-items: center;
        text-align: center;
    }

    .end-sars {
        color: #4B4848;        
        font-size: 2rem;
    }

    .aisha {
        width: 35%;
        /* height: 100%; */
    }

    .aisha img {
        width: 100%;
        height: 100%;
    }

    .it {
        width: 40%;
        display: flex;
        justify-content: space-evenly;
        background-color: #000000;
    }

    .rcc {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
    }

    .rcc-text {
        color: #B7A71B;
        font-size: 12px;
    }

    .it-text-div {
        display: flex;
        align-items: center;
    }

    .it-text {
        font-size: 85px;
        color: #B7A71B;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .it-text {
                font-size: 55px;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .it-text {
                font-size: 65px;
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

        @media only screen and (min-width: 1150px) {

            

        }       

    /* End of Responsive Styles */

</style>