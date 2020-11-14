<template>
    <div class="trending-topics" id="trendingTopics">
        <div class="trending-topics-label">
            <span class="label-title trending-topics-typography">Trending Topics</span>
            <div class="trending-topics-label-arrow-desktop">
                <span class="label-arrow-text trending-topics-typography">Trending Topics</span>
                <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
            </div>
        </div>
        <div class="trending-topics-body">
            <div class="trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/trending-topic-1.png" alt="trendingTopic1">
                </div>
                <span class="trending-topic-text trending-topics-typography">The protest continues</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
            <div class="trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/trending-topic-2.png" alt="trendingTopic2">
                </div>
                <span class="trending-topic-text trending-topics-typography">We must not give up now</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
            <div class="trending-topic last-trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/trending-topic-3.png" alt="trendingTopic3">
                </div>
                <span class="trending-topic-text trending-topics-typography tttm">What is the role of international communities on ENDSARS</span>
                <span class="trending-topic-text trending-topics-typography tttd">International Communities on Endsars</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
        </div>

        <!-- Desktop Template Markup -->

        <div class="trending-topics-body ttpb-desktop" id="ttpb-id-desktop">
            <div class="trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/patriotic.png" alt="trendingTopic4">
                </div>
                <span class="trending-topic-text trending-topics-typography">This would go into history book</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
            <div class="trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/lekki.png" alt="trendingTopic5">
                </div>
                <span class="trending-topic-text trending-topics-typography">Who ordered the lekki shooting?</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
            <div class="trending-topic last-trending-topic">
                <div class="trending-topic-img">
                    <img src="../assets/aisha-trending.png" alt="trendingTopic6">
                </div>
                <span class="trending-topic-text trending-topics-typography">Defend the future of Nigeria: Falz</span>
                <div class="trending-topic-video">
                    <img src="../assets/play-icon.png" alt="play-icon" class="trending-topic-play-icon">
                    <span class="trending-topic-video-text">We must not back down now: Youths</span>
                </div>
            </div>
        </div>

        <!-- End of Desktop Template Markup -->

        <div class="trending-topics-label-arrow-mobile">
            <span class="label-arrow-text trending-topics-typography">Trending Topics</span>
            <img src="../assets/right-arrow-icon.svg" alt="rightArrow" class="right-arrow">
        </div>
    </div>
</template>

<script>
export default {
    name: 'TrendingTopics'
}
</script>

<style scoped>


    /* Desktop Styles */

        @media screen and (min-width: 650px) {

            #trendingTopics {
                border-top: 0px solid #F6F6F6;
                border-radius: 0;
                box-shadow: 0 0 black;
            }

            .trending-topics .trending-topics-label-arrow-mobile, .tttm {
                display: none;
            }

            .trending-topics .trending-topics-label-arrow-desktop, .trending-topic .tttd {
                display: block;
            }

            .trending-topics .trending-topics-label {
                border-top: 1px solid #D0CDE1;
                border-bottom: 0;
                padding-left: 7%;
                padding-right: 7%;
                justify-content: space-between;
            }

            .trending-topics .trending-topics-label-arrow-desktop {
                display: flex;
                align-items: center;
                justify-content: space-between;
                width: 23%;
            }

            .trending-topics .trending-topics-label-arrow-desktop .label-arrow-text {
                color: #333333;
            }

            .trending-topics .trending-topics-body {
                flex-direction: row;
                width: 90%;
                margin: auto;
            }

            .trending-topics #ttpb-id-desktop {
                flex-direction: row;
                display: flex;
            }

            .trending-topics-body .last-trending-topic {
                border-bottom: 1px solid #00000029;
                margin-bottom: 1.5rem;
            }

            .trending-topics-body .trending-topic {
                /* height: 55vh; */
                flex-direction: column;
                width: 31%;
                padding-bottom: 0;
                justify-content: space-around;
            }

            #ttpb-id-desktop .trending-topic {
                border-bottom: 0;
            }

            .trending-topic .trending-topic-img {
                width: 100%;
            }

            .trending-topic .trending-topic-text {
                width: 100%;
                margin: 1rem 0;
                margin-left: 15%;
            }

            .trending-topic .trending-topic-img img {
                border-bottom: 5px solid #46E146;
            }

            .trending-topic .trending-topic-video {
                display: flex;
                align-items: center;
                margin-bottom: 0.7rem;
            }

            .trending-topic-video-text {
                font-size: 14px;
                margin-left: 5%;
            }

            .trending-topic-play-icon {
                background-color: #B9D4B9;
                width: 9%;
                border-radius: 50%;
                padding: 5px;
            }

        }

    /* End of Desktop Styles */

    .trending-topics-typography {
        font-family: Georgia, 'Times New Roman', Times, serif;
    }

    .trending-topics {
        border-top: 7px solid #46E146;
        margin-top: 3rem;
        border-radius: 16px;
        box-shadow: 0 3px 6px #00000029;
    }

    .trending-topics-label {
        display: flex;
        border-bottom: 1px solid #D0CDE1;
        padding: 2rem 0;
        margin-bottom: 1.5rem;
        padding-left: 10%;
    }

    .trending-topics-label-arrow-desktop, .trending-topics .ttpb-desktop, .trending-topic-video, .tttd {
        display: none;
    }

    .trending-topics-label-arrow-mobile {
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 28%;
        margin-left: 65%;
        padding-bottom: 1.5rem;
    }

    .label-title {
        color: #333333;
        font-weight: bold;
        font-size: 20px;
    }

    .label-arrow-text {
        color: #46E146;
        font-weight: bold;
        font-size: 12px;
    }

    .trending-topics-body {
        display: flex;
        flex-direction: column;
    }

    .trending-topic {
        display: flex;
        justify-content: space-between;
        width: 85%;
        margin: auto;
        border-bottom: 1px solid #00000029;
        margin-bottom: 1.5rem;
        padding-bottom: 1rem;
    }

    .last-trending-topic {
        border-bottom: 0px;
        margin-bottom: 1rem;
    }

    .trending-topic-img {
        width: 50%;
    }

    .trending-topic-img img {
        width: 100%;
        height: 100%;
        border-radius: 16px;
    }

    .trending-topic-text {
        width: 45%;
        color: #333333;
        font-size: 16px;
        align-self: center;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .trending-topics-label-arrow-mobile {
                width: 45%;
                margin-left: 50%;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .trending-topics-label-arrow-mobile {
                width: 40%;
                margin-left: 55%;
            }

        }

        @media only screen and (max-width: 550px) and (min-width: 450px) {

            .trending-topics-label-arrow-mobile {
                width: 35%;
                margin-left: 55%;
            }

        }

        @media only screen and (max-width: 1050px) and (min-width: 950px) {

            

        }

        @media only screen and (max-width: 1150px) and (min-width: 1050px) {

            

        }

        @media only screen and (min-width: 1150px) {

            .trending-topic-play-icon {
                width: 5%;
            }
            
        }

        @media only screen and (max-width: 1150px) and (min-width: 1050px) {

            

        } 

        @media only screen and (min-width: 1150px) {

            

        }       

    /* End of Responsive Styles */

</style>