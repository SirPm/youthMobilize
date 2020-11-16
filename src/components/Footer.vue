<template>
    <footer id="footer">
        <div class="footer">
            <div class="footer-links">
                <div class="upper-footer-links">
                    <div class="footer-link-div">
                        <span class="heading">Home</span>
                        <ul class="footer-links-div">
                            <li><a href="!#" class="footer-link">Trending</a></li>
                            <li><a href="!#" class="footer-link">Communities</a></li>
                            <li><a href="!#" class="footer-link">Meet the Law</a></li>
                            <li><a href="!#" class="footer-link">Health Tips</a></li>
                            <li><a href="!#" class="footer-link">Our Team</a></li>
                            <li><a href="!#" class="footer-link">Press</a></li>
                            <li><a href="!#" class="footer-link">Partners</a></li>
                        </ul>
                    </div>
                    <div class="footer-link-div">
                        <span class="heading">Communities</span>
                        <ul class="footer-links-div">
                            <li><a href="!#" class="footer-link">Nigerian Youths</a></li>
                            <li><a href="!#" class="footer-link">Nigerians in diaspora</a></li>
                            <li><a href="!#" class="footer-link">Tech & Innovations</a></li>
                            <li><a href="!#" class="footer-link">Entertainment</a></li>
                            <li><a href="!#" class="footer-link">The Lawyers</a></li>
                            <li><a href="!#" class="footer-link">Medical Community</a></li>
                            <li><a href="!#" class="footer-link">Sport</a></li>
                        </ul>
                    </div>
                    <div class="footer-link-div">
                        <span class="heading">Sales</span>
                        <ul class="footer-links-div">
                            <li><a href="!#" class="footer-link">123-456-789</a></li>
                            <li><a href="!#" class="footer-link">Contact Sales</a></li>
                            <li><a href="!#" class="footer-link">Pricing & Plan</a></li>
                            <li><a href="!#" class="footer-link">Request a Demo</a></li>
                            <li><a href="!#" class="footer-link">Webinars & Events</a></li>
                            <li><a href="!#" class="footer-link">Blog</a></li>
                            <li><a href="!#" class="footer-link">Site Map</a></li>
                        </ul>
                    </div>
                </div>
                <div class="lower-footer-links">
                    <div class="footer-link-div">
                        <span class="heading">Support</span>
                        <ul class="footer-links-div">
                            <li><a href="!#" class="footer-link">FAQ</a></li>
                            <li><a href="!#" class="footer-link">Job</a></li>
                            <li><a href="!#" class="footer-link">Feedback</a></li>
                            <li><a href="!#" class="footer-link">Accessibility</a></li>
                            <li><a href="!#" class="footer-link">Privacy & Security</a></li>
                            <li><a href="!#" class="footer-link">Support Center</a></li>
                        </ul>
                    </div>
                    <div class="footer-lang-and-social">
                        <span class="heading">Language</span>
                        <select class="select-lang">
                            <option>English</option>
                            <option>French</option>
                        </select>
                        <div class="social-icons">
                            <img src="../assets/insta-icon.svg" alt="insta" class="social-icon">
                            <img src="../assets/twitter-icon.svg" alt="twitter" class="social-icon">
                            <img src="../assets/fb-icon.svg" alt="fb" class="social-icon">
                            <img src="../assets/earth.svg" alt="earth" class="social-icon">
                        </div>
                    </div>
                </div>
            </div>
            <div class="footer-ending">
                <span class="rights">All Rights Reserved, &copy; 2020 YouthMobilize</span>
                <div class="terms-privacy-cookies">
                    <span class="tpc">Terms of Service</span>
                    <span class="tpc">Privacy</span>
                    <span class="tpc">Cookies</span>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style scoped>

    /* Desktop Styles */

        @media screen and (min-width: 650px) {
            
            #footer {
                margin-top: 10rem;
            }

            #footer .footer {
                width: 80%;
            }

            .footer .footer-links {
                flex-direction: row;
                height: auto;
                padding-bottom: 1rem;
            }

            .footer-links .upper-footer-links {
                width: 60%;
            }

            .footer-links .lower-footer-links {
                width: 35%;
                margin-top: 0;
            }

            .lower-footer-links .footer-link-div, .lower-footer-links .footer-lang-and-social {
                width: 47%;
            }

            .footer-lang-and-social .heading {
                width: fit-content;
            }

            .footer-lang-and-social .select-lang {
                color: #ffffff;
                background-color: #B7A71B;
            }

            .footer-lang-and-social .social-icons {
                margin-bottom: 2.5rem;
            }

            .social-icons .social-icon {
                width: 15%;
            }

            .footer .footer-ending {
                display: flex;
                justify-content: space-between;
            }

            .footer-ending .terms-privacy-cookies {
                width: 30%;
            }

        }

    /* End of Desktop Styles */

    footer {
        margin-top: 4rem;
        background-color: #0F6D0F;
        color: #ffffff;
        position: relative;
    }

    .footer {
        width: 95%;
        margin: auto;
        padding-bottom: 3rem;
    }

    .heading {
        font-size: 16px;
        display: inline-block;
        margin-bottom: 1rem;
    }

    .footer-links {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding-top: 3rem;
    }

    .upper-footer-links, .lower-footer-links {
        display: flex;
        justify-content: space-between;
    }

    .lower-footer-links {
        margin-top: 3rem;
    }

    .footer-links-div {
        list-style: none;
    }

    .footer-links-div li {
        margin-bottom: 0.5rem;
    }

    .footer-link {
        text-decoration: none;
        color: #ffffff;
        font-size: 12px;
    }

    .footer-lang-and-social {
        display: flex;
        flex-direction: column;
        width: 50%;
        margin-right: 10%;
        height: fit-content;
    }

    .select-lang {
        width: fit-content;
        padding: 10px;
        font-size: 11px;
        color: #34B434;
        font-weight: bold;
        /* margin-bottom: 35px; */
    }

    .social-icons {
        display: flex;
        justify-content: space-between;
    }

    .social-icon {
        width: 10%;
    }

    .social-icon img {
        width: 100%;
    }

    .earth-icon {
        display: flex;
    }

    .horizontal-rule {
        background-color: #DCD5CB;
        position: absolute;
        width: 100%;
        left: 0;
        bottom: 6.5rem;
    }

    .footer-ending {
        margin-top: 35px;
        font-size: 12px;
    }

    .rights {
        display: inline-block;
        margin-bottom: 1rem;
    }

    .terms-privacy-cookies {
        display: flex;
        justify-content: space-between;
        width: 60%;
    }


    /* Responsive Styles */

        @media only screen and (max-width: 350px) and (min-width: 300px) {

            .heading {
                font-size: 12px;
            }

            .footer-link {
                font-size: 10px;
            }

            .footer-lang-and-social {
                width: 40%;
            }

            .social-icon {
                width: 20%;
            }

            .terms-privacy-cookies {
                width: 100%;
            }

        }

        @media only screen and (max-width: 450px) and (min-width: 350px) {

            .heading {
                font-size: 14px;
            }

            .footer-link {
                font-size: 11px;
            }

            .footer-lang-and-social {
                width: 35%;
            }

            .social-icon {
                width: 20%;
            }

            .terms-privacy-cookies {
                width: 80%;
            }

        }

        @media only screen and (max-width: 650px) and (min-width: 450px) {

            .footer-ending .terms-privacy-cookies {
                width: 50%;
            }

        }

        @media only screen and (max-width: 750px) and (min-width: 650px) {

            .footer-ending .terms-privacy-cookies {
                width: 40%;
            }

        }

    /* End of Responsive Styles */

</style>