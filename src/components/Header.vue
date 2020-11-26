<template>
    <header class='header'>

        <!-- Desktop Template Markup -->

        <div class="desktop-header">
            <img src="../assets/youth-mobilize-logo.png" alt="youthMobilize" class="desktop-youth-mobilize-logo">
            <div class="desktop-header-inner">
                <ul class="desktop-links">
                    <li class="desktop-link-item desktop-link-item-home">
                        <div class="home" v-bind:class="{ currentPageIconStyle : currentPageIconStatus }"><img src="../assets/homeIcon.svg" alt="homeIcon" class="home-icon"></div>
                        <!-- make more research on how you can make the current routed page have its corresponding header link hover styles visible -->
                        <a href="!#" class="desktop-link" v-bind:class="{ currentPageStyle : currentPageStatus }">Home</a>
                    </li>
                    <li class="desktop-link-item">
                        <div class="trending"><img src="../assets/trending-icon-50.png" alt="trendingIcon" class="dli-icon"></div>
                        <a href="!#" class="desktop-link">Trending</a>
                    </li>
                    <li class="desktop-link-item">
                        <div class="communities"><img src="../assets/communities-icon.png" alt="communitiesIcon" class="dli-icon"></div>
                        <div class="dli-sub">
                            <span class="desktop-link">Communities</span>
                            <!-- <img src="../assets/caret.png" alt="caretIcon" class="caret-icon" @click="toggleSubLinksCommunity"> -->
                        </div>
                        <ul class="sub-desktop-links" v-bind:class="{ showSubDesktopLinks : subDesktopLinksStatusCommunity }">
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Nigerian Youths</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Nigerians in Diaspora</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Tech & Innovations</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Entertainment</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">The Lawyers</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Medical Team</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Sports</a></li>
                        </ul>
                    </li>
                    <li class="desktop-link-item">
                        <div class="more"><img src="../assets/more-icon.svg" alt="moreIcon" class="dli-icon"></div>
                        <div class="dli-sub">
                            <span class="desktop-link">More</span>
                            <!-- <img src="../assets/caret.png" alt="caretIcon" class="caret-icon" @click="toggleSubLinksMore"> -->
                        </div>
                        <ul class="sub-desktop-links" v-bind:class="{ showSubDesktopLinks : subDesktopLinksStatusMore }">
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Post Articles</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Jobs</a></li>
                            <li class="sub-desktop-link-item"><a href="!#" class="sub-desktop-link">Contact Us</a></li>
                        </ul>
                    </li>
                </ul>
                <div class="desktop-sign-in-search-and-text">
                    <div class="sign-in-and-search">
                        <a href="!#" class="sign-up">Sign up</a>
                        <a href="!#" class="login">Login</a>
                        <img class="desktop-search-icon" src="../assets/search-icon.svg" alt="search-icon">
                    </div>
                    <div class="text">End Police Brutality</div>
                </div>
            </div>
        </div>

        <!--End of Desktop Template Markup -->

        <!-- Mobile Template Markup -->

        <div class="youth-mobilize-logo-div">
            <img class="youth-mobilize-logo" src="../assets/youth-mobilize-logo.png" alt="youthMobilize">
        </div>
        <div class="header-icons-div">
            <img class="person-icon" src="../assets/person-icon.svg" alt="person-icon">
            <img class="search-icon" src="../assets/search-icon.svg" alt="search-icon">
            <div class="menu-btn" v-bind:class="{ close: isClose }" @click="toggleMenu">
                <span class="menu-btn__burger" v-bind:class="{ open: isOpen }"></span>
            </div>
        </div>

        <nav class="nav" v-bind:class="{ open: isOpen }">
            <ul class="menu-nav" v-bind:class="{ open: isOpen }">
                <li class="menu-nav__item active" v-bind:class="{ open: isOpen }">
                    <span class="menu-nav__link">Youth Mobilize</span>
                    <ul class="sub-menu-nav">
                        <li class="sub-menu-nav__item">
                            <a href="!#" class="sub-menu-nav__link">Home</a>
                        </li>
                        <li class="sub-menu-nav__item">
                            <a href="!#" class="sub-menu-nav__link">Trending</a>
                        </li>
                        <li class="sub-menu-nav__item">
                            <a href="!#" class="sub-menu-nav__link">Communities</a>
                        </li>
                        <li class="sub-menu-nav__item">
                            <a href="!#" class="sub-menu-nav__link">Jobs</a>
                        </li>
                    </ul>
                </li>
                <li class="menu-nav__item" v-bind:class="{ open: isOpen }">
                    <a href="!#" class="menu-nav__link">Top Videos</a>
                </li>
                <li class="menu-nav__item" v-bind:class="{ open: isOpen }">
                    <a href="!#" class="menu-nav__link">Login / Sign up</a>
                </li>
                <li class="menu-nav__item" v-bind:class="{ open: isOpen }">
                    <a href="!#" class="menu-nav__link">Contact Us</a>
                </li>
                <li class="menu-nav__item" v-bind:class="{ open: isOpen }">
                    <a href="!#" class="menu-nav__link">Log Out</a>
                </li>
            </ul>
        </nav>

        <!--End of Mobile Template Markup -->
    </header>
</template>

<script>

export default {
    name: 'Header',
    data() {
        return {
            isOpen: false,
            isClose: false,
            subDesktopLinksStatusCommunity: false,
            subDesktopLinksStatusMore: false,
            currentPageStatus: true,
            currentPageIconStatus: true
        }
    },
    methods: {
        toggleMenu() {
            if (!this.isOpen) {
                this.isOpen = true;
                this.isClose = true;
            } else {
                this.isOpen = false;
                this.isClose = false;
            }
        },
        toggleSubLinksCommunity() {
            if(!this.subDesktopLinksStatusCommunity) {
                this.subDesktopLinksStatusCommunity = true;
            } else {
                this.subDesktopLinksStatusCommunity = false;
            }
        },
        toggleSubLinksMore() {
            if(!this.subDesktopLinksStatusMore) {
                this.subDesktopLinksStatusMore = true;
            } else {
                this.subDesktopLinksStatusMore = false;
            }
        }
    }
} 
</script>

<style scoped>

    .header {
        width: 100%;
        height: fit-content;
        display: flex;
        box-shadow: 0 3px 6px #00000029;
        /* position: relative; */
        position: fixed;
        top: 0;
        z-index: 600;
    }

    ul {
        list-style: none;
    }

    a {
        text-decoration: none;
    }

    /* Desktop Styles */

    @media screen and (min-width: 650px) {

        .header .header-icons-div, .youth-mobilize-logo-div {
            display: none;
        }

        .header .desktop-header {
            background-color: #0F6D0F;
            width: 100vw;
            display: flex;
        }

        .header .desktop-header .desktop-header-inner {
            width: 96%;
            /* margin: auto; */
            display: flex;
            justify-content: space-between;
            margin-right: 2%;
        }

        .desktop-youth-mobilize-logo {
            width: 13%;
            background-color: #B9D4B9;
            padding: 12px 20px;
            padding-top: 20px;
        }

        .desktop-links {
            list-style: none;
            display: flex;
            align-items: center;
            width: 50%;
            position: relative;
            margin-left: 10%;
        }

        .desktop-link-item {
            width: 20%;
            display: flex;
            align-items: center;
            flex-direction: column;
            /* margin-bottom: 1.1rem; */
        }

        .desktop-link-item-home {
            width: 15%;
            align-items: flex-end;
        }

        /* .desktop-link-item:nth-child(3) {
            margin-right: 10%;
        } */

        .desktop-link-item:nth-child(3) .dli-sub .caret-icon {
            width: 10%;
        }

        .home, .trending, .communities, .more {
            display: none;
        }

        /* .desktop-link-item:hover > .home, .desktop-link-item:hover > .trending, .desktop-link-item:hover > .communities, .desktop-link-item:hover > .more, .currentPageIconStyle {
            display: block;
        } */



        /* .desktop-link-item:hover > .desktop-link, .desktop-link-item:hover > .dli-sub > .desktop-link, .currentPageStyle {
            border-bottom: 3px solid #46E146;
            padding-bottom: 30px;
            border-radius: 3px;
        } */

        /* .currentPageIconStyle {
            display: block;
        } */

        .currentPageStyle {
            border-bottom: 4px solid #46E146;
            padding-top: 31px;
            padding-bottom: 25px;
            border-radius: 3px;
        }

        .sub-desktop-links {
            position: absolute;
            top: 100%;
            background-color: #D0CDE1;
            padding: 10px 15px;
            border-radius: 10px;
            flex-direction: column;
            align-items: center;
            display: none;
        }

        .showSubDesktopLinks {
            display: flex;
        }

        .sub-desktop-link-item {
            margin-bottom: 0.5rem;
        }

        .sub-desktop-link {
            color: #000000;
            font-size: 12px;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        /* border-bottom: 5px solid #46E146; */

        .home-icon {
            width: 15%;
            /* display: inline-block; */
            margin-left: 70%;
        }

        .communities .dli-icon {
            margin-left: 20%;
        }

        .dli-icon {
            width: 25%;
            display: inline-block;
            margin-left: 43%;
        }

        .more {
            margin-right: 40%;
        }

        .more .dli-icon {
            width: 55%;
            margin-left: 0;
        }

        .dli-sub {
            display: flex;
        }

        .caret-icon {
            width: 15%;
            display: inline-block;
            margin-left: 5%;
            align-self: center;
            cursor: pointer;
        }

        .desktop-link {
            text-decoration: none;
            color: #ffffff;
            font-size: 11px;
            text-transform: uppercase;
            align-self: center;
        }

        .desktop-sign-in-search-and-text {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            width: 25%;
            padding-top: 1%;
        }

        .sign-in-and-search {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .desktop-search-icon {
            border-left: 2px solid #B9D4B9;
            padding-left: 10%;
            height: 4vh;
            width: 23%;
        }

        .sign-up, .login, .text {
            font-weight: bold;
            color: #ffffff;
            font-family: Helvetica, sans-serif;
        }

        .sign-up, .login {            
            font-size: 11px;
            text-transform: uppercase;
        }

        .login {
            border-left: 2px solid #B9D4B9;
            padding-left: 15%;
            height: 4vh;
            display: flex;
            align-items: center;
        }

        .text {
            font-size: 16px;
            border-left: 2px solid #B9D4B9;
            padding-left: 10%;
            margin-top: 8%;
        }

    }

    /* End of Desktop Styles */


    /* Mobile Styles */

    .desktop-header {
        display: none;
    }

    .youth-mobilize-logo-div {
        width: 20%;
        z-index: 600;
        position: relative;
        background-image: linear-gradient( to right, #DEFFDE, #ECECEC );
    }

    .youth-mobilize-logo {
        width: 100%;
        height: 100%;
        background-color: #00000029;
        padding: 10px;
    }

    .person-icon {
        margin-left: 63%;
        border-right: 1px solid #B9D4B9;
        border-left: 1px solid #B9D4B9;
        width: 12%;
        /* padding: 5px;
        padding-right: 10px; */
        padding: 3px;
        height: 25px;
    }

    .search-icon {
        /* margin-left: 2%; */
        border-right: 1px solid #B9D4B9;
        width: 12%;
        /* padding: 5px;
        padding-right: 10px; */
        padding: 3px;
        height: 25px;
    }

    .header-icons-div {
        background-color: #0F6D0F;
        width: 80%;
        display: flex;
        align-items: center;
    }

    .menu-btn {
        position: absolute;
        top: 1.34rem;
        right: 1rem;
        width: 20px;
        height: 20px;
        z-index: 1;
        cursor: pointer;
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
    }

    .menu-btn.close {
        background-color: red;
        top: 0;
        right: 0;
        width: 9vw;
        height: 100%;
    }

    .menu-btn__burger {
        width: 20px;
        height: 2px;
        background-color: #ffffff;
        position: absolute;
        top: 0.5rem;
        right: 0;
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
        border-radius: 5px;
    }

    .menu-btn__burger::before {
        content: '';
        width: 20px;
        top: -8px;
        height: 2px;
        background-color: #ffffff;
        position: absolute;
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
        border-radius: 5px;
    }

    .menu-btn__burger::after {
        content: '';
        width: 20px;
        top: 8px;
        height: 2px;
        background-color: #ffffff;
        position: absolute;
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
        border-radius: 5px;
    }

    .menu-btn__burger.open {
        -webkit-transform: rotate(720deg);
        transform: rotate(720deg);
        background: transparent;
        top: 45%;
        right: 20%;
    }

    .menu-btn__burger.open::before {
        -webkit-transform: rotate(45deg) translate(5px, 8px);
        transform: rotate(45deg) translate(5px, 8px);
    }

    .menu-btn__burger.open::after {
        width: 20px;
        -webkit-transform: rotate(-45deg) translate(3px, -7px);
        transform: rotate(-45deg) translate(3px, -7px);
    }


    .nav {
        position: fixed;
        top: 10vh;
        left: 0;
        width: 50vw;
        opacity: 0.98;
        visibility: hidden;
    }

    .nav.open {
        visibility: visible;
    }

    .nav .menu-nav {
        height: 90vh;
        background-color: #3b5a3b;
        list-style: none;
        -webkit-transform: translateX(-100%);
        transform: translateX(-100%);
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
    }

    .nav .menu-nav.open {
        -webkit-transform: translateX(0);
        transform: translateX(0);
    }

    .nav .menu-nav__item {
        -webkit-transition: 0.5s ease-in-out;
        transition: 0.5s ease-in-out;
    }

    .nav .menu-nav__item.open {
        border-bottom: 1px solid #D0CDE1;
        display: flex;
        align-items: center;
        background-color: #34B434;
    }

    .nav .menu-nav__link {
        display: inline-block;
        font-weight: 300;
        font-size: 1.2rem;
        transition: 0.5s ease-in-out;
        color: #ffffff;
        text-decoration: none;
        padding: 2rem 0;
        width: 100%;
        height: 100%;
        padding-left: 10%;
    }

    .sub-menu-nav {
        position: absolute;
        left: 100%;
        display: flex;
        width: 50vw;
        flex-flow: column wrap;
        background-color: #ffffff;
        top: 0;
        transition: 0.5s ease-in-out;
        display: none;
    }

    .nav .menu-nav .menu-nav__item:hover .sub-menu-nav, .menu-nav__link:hover {
        background-color: #C6F3C6;
        color: #484848;
        display: block;
    }

    .sub-menu-nav::before {
        content: "";
        position: absolute;
        top: 25px;
        left: -30px;
        z-index: 1;
        border: 15px solid;
        border-color: transparent #ffffff transparent transparent;
    }

    .sub-menu-nav__item {
        list-style: none;
        transform: translateX(0);
        border-bottom: 1px solid #D0CDE1;
        display: flex;
        align-items: center;
        background-color: #ffffff;
        padding: 1rem;
    }

    .sub-menu-nav__link {
        text-decoration: none;
        color: #484848;
        font-weight: bold;
        display: inline-block;
        margin-left: 10%;
        font-weight: 600;
        font-size: 1.2rem;
        transition: 0.5s ease-in-out;
        padding: 1rem 0;
    }

    .menu-nav__item:nth-child(1) {
        -webkit-transition-delay: 0.25s;
        transition-delay: 0.25s;
    }

    .menu-nav__item:nth-child(2) {
        -webkit-transition-delay: 0.35s;
        transition-delay: 0.35s;
    }

    .menu-nav__item:nth-child(3) {
        -webkit-transition-delay: 0.45s;
        transition-delay: 0.45s;
    }

    .menu-nav__item:nth-child(4) {
        -webkit-transition-delay: 0.55s;
        transition-delay: 0.55s;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .person-icon {
                margin-left: 51%;
                width: 15%;
            }

            .search-icon {
                width: 15%;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .person-icon {
                margin-left: 58%;
                width: 13%;
            }

            .search-icon {
                width: 13%;
            }

        }

        @media only screen and (max-width: 650px) and (min-width: 500px) {

            .person-icon {
                margin-left: 68%;
                width: 10%;
            }

            .search-icon {
                width: 10%;
            }

        }

        @media only screen and (max-width: 950px) and (min-width: 650px) {

            .home-icon {
                width: 25%;
                margin-left: 55%;
            }

        }

        @media only screen and (max-width: 1050px) and (min-width: 650px) {

            .desktop-links {
                width: 60%;
            }

            .desktop-link-item {
                width: 40%;
            }

            .desktop-link-item-home {
                width: 15%;
            }

        }

        @media only screen and (max-width: 650px) and (min-width: 200px) {

            .header {
                height: 59px;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 400px) {

            .person-icon {
                margin-left: 60%;
            }
        } 

        @media only screen and (max-width: 350px) and (min-width: 300px) {
            .menu-btn.close {
                width: 14vw;
            }
        }
         
        @media only screen and (max-width: 400px) and (min-width: 350px) {
            .menu-btn.close {
                width: 11vw;
            }
        }

        @media only screen and (max-width: 500px) and (min-width: 400px) {
            .menu-btn.close {
                width: 10vw;
            }
        }


        @media only screen and (max-width: 650px) and (min-width: 300px) {
            .nav .menu-nav {
                height: 91vh;
                margin-top: -8px;
            }
        }

        @media only screen and (min-width: 935px) {

            .text {
                margin-left: 14%;
            }

        } 

        @media only screen and (min-width: 1050px) {

            .desktop-search-icon {
                width: 18%;
            }

        }       

    /* End of Responsive Styles */


</style>