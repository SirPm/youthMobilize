<template>
    <div class="endsars-videos">
        <div class="endsars-videos-inner">
            <div class="endsars-video">
                <img src="../assets/Endsars1.png" alt="endsars1">
                <img src="../assets/play-grey.png" alt="play-icon" class="related-content-play-icon" id="playIcon">
                <div class="top-videos-div">
                    <h3 class="top-videos-title">Top Videos</h3>
                    <p class="top-videos-paragraph">The most recent event videos across the Country on Police brutality and extortions</p>
                    <h5 class="related-content-title">Related content</h5>
                    <div class="related-content-div">
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">Abuja protest hijacked by political thugs</span>
                        </div>
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">Unnamed Federal Senator behind Abuja hijacked protest</span>
                        </div>
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">Police PPRO promise immediate end to SARS but came up with SWAT</span>
                        </div>
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">Lagos protest as its becoming more interesting</span>
                        </div>
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">The world should learn from this kind of peaceful protest</span>
                        </div>
                        <div class="related-content-item">
                            <img src="../assets/play-icon.png" alt="play-icon" class="related-content-play-icon">
                            <span class="related-content-text">CP Nwanfo on the run!</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="endsars-videos-list">
                <div class="endsars-videos-list-item mb">
                    <div class="video-list-item-img">
                        <img src="../assets/candle-night.png" alt="candleLight">
                    </div>
                    <div class="video-info">
                        <span class="video-title endsars-video-text-typography">End Sars</span>
                        <span class="video-text endsars-video-text-typography">Candle light held for the stained</span>
                    </div>
                </div>
                <div class="endsars-videos-list-item mt">
                    <div class="video-list-item-img">
                        <img src="../assets/lekki-shooting.png" alt="lekkiShooting">
                    </div>
                    <div class="video-info">
                        <span class="video-title endsars-video-text-typography">Lekki Shooting</span>
                        <span class="video-text endsars-video-text-typography">Who ordered the shooting?: Nigerian youths demands justice for those killed.</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'EndSarsVideo'
}
</script>

<style scoped>

    /* Desktop Styles */

        @media screen and (min-width: 650px) {
            
            .endsars-videos {
                display: flex;
                flex-direction: column;
            }

            .endsars-videos-inner {
                background-image: linear-gradient( to right, #DEFFDE, #A9F8A9, #A0E3A0, #ECECEC );
                padding: 2rem 0;
            }

            .endsars-videos .endsars-video {
                display: flex;
                justify-content: space-between;
                width: 96%;
                height: 350px;
                background-color: #ffffff;
                z-index: 100;
            }

            .endsars-videos .endsars-video .related-content-play-icon {
                background-color: #B9D4B9;
                width: 6%;
                border-radius: 50%;
                padding: 5px;
            }

            .endsars-video #playIcon {
                width: 5%;
                right: 75%;
            }

            .endsars-video .top-videos-div {
                display: flex;
                flex-direction: column;
                /* justify-content: space-evenly; */
                justify-content: space-between;
                color: #ffffff;
                background-color: #0F6D0F;
                width: 49.5%;
                padding: 10px 20px;
            }

            .top-videos-title {
                font-family: Georgia, 'Times New Roman', Times, serif;
                font-size: 30px;
                font-weight: bold;
                /* margin-bottom: 20px; */
            }

            /* .related-content-title {
                margin: 10px 0;
            } */

            .top-videos-paragraph {
                font-size: 14px;
            }

            .endsars-videos .endsars-video img {
                width: 49.5%;
            }

            .related-content-text {
                font-size: 14px;
                margin-left: 2%;
            }

            .related-content-item {
                display: flex;
                align-items: center;
                margin-bottom: 8px;
            }

            .endsars-videos-inner .endsars-videos-list-item {
                width: 49.5%;
                margin: 0;
            }

            .endsars-videos-list-item .video-info {
                width: 73.3%;
            }

            .endsars-videos-inner .endsars-videos-list {
                flex-direction: row;
                width: 96%;
                margin: auto;
                box-shadow: 0 0 0 white;
                background-image: linear-gradient(45deg, transparent, transparent);
                background: white;
                padding-bottom: 0;
                justify-content: space-between;
                padding-top: 14px;
            }

            .endsars-videos-list .pb, .endsars-videos-list .pt {
                padding: 0;
            }

        }


    /* End of Desktop Styles */

    .endsars-video-text-typography {
        color: #ffffff;
    }

    .top-videos-div {
        display: none;
    }

    .endsars-videos {
        margin-top: 3rem;
    }

    .endsars-video {
        width: 96%;
        margin: auto;
        position: relative;
        z-index: -300;
    }

    #playIcon {
        position: absolute;
        width: 9%;
        border-radius: 50%;
        padding: 10px;
        top: 50%;
        right: 50%;
        background-color: #ffffff;
    }

    .endsars-video img {
        width: 100%;
    }

    .endsars-videos-list {
        display: flex;
        flex-direction: column;
        background-image: linear-gradient( to right, #DEFFDE, #A9F8A9, #A0E3A0, #ECECEC );
        box-shadow: 0 3px 6px #00000029;
        padding: 40px 0;
    }

    .endsars-videos-list-item {
        width: 96%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        background-color: #ffffff;
    }

    .mb {
        margin-bottom: 5px;
    }

    .mt {
        margin-top: 5px;
    }

    .video-list-item-img {
        width: 25%;
    }

    .video-list-item-img img {
        width: 100%;
        height: 100%;
    }

    .video-info {
        background-color: #0F6D0F;
        width: 73.8%;
        display: flex;
        flex-direction: column;
        /* justify-content: space-around; */
        padding-left: 15px;
        padding-top: 5%;
    }

    .video-title {
        font-style: italic;
        font-weight: bold;
        font-size: 11px;
    }

    .video-text {
        font-size: 12px;
        margin-top: 3%;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            

        }

        @media only screen and (max-width: 550px) and (min-width: 450px) {

            #playIcon {
                width: 7%;
            }

        }

        @media only screen and (max-width: 650px) and (min-width: 550px) {

            #playIcon {
                width: 7%;
            }

        }

        @media only screen and (max-width: 1150px) and (min-width: 950px) {

            /* .endsars-video #playIcon {
                width: 4%;
            } */

            .endsars-videos .endsars-video .related-content-play-icon {
                width: 5%;
            }

        }

        @media only screen and (max-width: 1150px) and (min-width: 850px) {

            /* .endsars-video .top-videos-div {
                padding: 0 20px;
            } */

        } 

        @media only screen and (min-width: 1150px) {

            /* .endsars-video #playIcon {
                width: 3%;
            } */

            .endsars-videos .endsars-video .related-content-play-icon {
                width: 4%;
            }

            /* .endsars-videos .endsars-video {
                height: 350px;
            } */

            /* .endsars-video .top-videos-div {
                padding: 10px 20px;
            } */

        }       

    /* End of Responsive Styles */

</style>