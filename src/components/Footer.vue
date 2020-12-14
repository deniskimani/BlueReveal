<template>
    <div :class="`footer ${$route.name == 'contact'  || $route.name == 'services' || $route.name == 'about' ? 'borders' : '' }`">
        <div class="container">
            <div class="row">
                <div class="col-md-3">
                    <div class="footer-logo mb-4 text-center">
                        <img src="/img/bluereveal-blue.png"  alt="logo">
                    </div>
                    <p>A software company that cares about your needs.</p>
                </div>
                <div class="col-md-3">
                    <h3>Contact Info</h3>
                    <ul>
                    <li>
                    <p><a>Address : Nairobi, Kenya</a></p>
                    </li>
                    <li>
                    <p><a>Phone : +254 (725) 883 727</a></p>
                    </li>
                    <li>
                    <p><a>Email : info@bluereaveal.co.ke</a></p>
                    </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h3>Useful Links</h3>
                    <ul>
                    <li>
                    
                    <router-link :to="{name : 'services'}">Services</router-link>
                    </li>
                    <li>
                    <router-link :to="{name : 'about'}">About Us</router-link>
                    </li>
                    <li>
                    <router-link :to="{name : 'contact'}">Contact Us</router-link>
                    </li>
                    <li>
                    <router-link :to="{name : 'portfolio'}">Portfolio</router-link>
                    </li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h3>Newsletter & Social Media</h3>
                    
                    <div class="newsletter">
                        <input type="email"  name="email" placeholder="Enter your Email Address">
                        <a href=""><span class="fa fa-paper-plane-o" aria-hidden="true"></span></a>
                    </div>
                    <p>Subscribe to our newsletter.</p>
                    <div class="socials">
                        <a href=""><span><i class="fa fa-facebook-official" aria-hidden="true"></i></span></a>
                        <a href=""><span><i class="fa fa-twitter" aria-hidden="true"></i></span></a>
                        <a href=""><span><i class="fa fa-google-plus-square" aria-hidden="true"></i></span></a>
                        <a href=""><span><i class="fa fa-instagram" aria-hidden="true"></i></span></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style lang="scss" scoped>
.footer {
    padding-top: 50px;
    padding-bottom: 50px;
    .socials {
        padding-top: 20px;
        .fa-facebook-official {
            font-size: 24px;
            padding: 0 10px;
            &:hover {
                color: rgb(54, 78, 129)
            }
        }
        .fa-twitter {
            font-size: 24px;
            padding: 0 10px;
            &:hover {
                color: rgb(61, 242, 255)
            }
        }
        .fa-google-plus-square {
            font-size: 24px;
            padding: 0 10px;
            &:hover {
                color: rgb(253, 70, 14)
            }
        }
        .fa-instagram {
            font-size: 24px;
            padding: 0 10px;
            &:hover {
                color: rgb(150, 27, 27)
            }
        }
    }
    h3 {
        font-family: poppins, sans-serif;
        font-size: 18px;
        margin-bottom: 30px;
        font-weight: 600;
        color: #464545;
    }
    ul {
        list-style: none;
        padding-left: 0;

        li {
            padding: 2px 0;

            a {
                color: #7f7f7f !important;
                margin-bottom: 10px;
                display: inline-block;
            }
        }
    }
    .newsletter {
        input {
            height: 48px;
            border-radius: 30px;
            border-top-right-radius: 0;
            border-bottom-right-radius: 0;
            padding-left: 17px;
            width: 200px;
            border-left: none !important;
            outline: none;
        }
        a {
            span {
                height: 50px !important;
                border: 1px solid #e9e7ec;
                line-height: 46px;
                width: 46px;
                border-radius: 30px;
                border-bottom-left-radius: 0;
                border-top-left-radius: 0;
                padding-left: 7px;
                color: #fff;
                background: #0ab6ff;
            }
    
            span:hover {
                height: 50px !important;
                border: 1px solid #e9e7ec;
                line-height: 46px;
                width: 46px;
                border-radius: 30px;
                border-bottom-left-radius: 0;
                border-top-left-radius: 0;
                padding-left: 7px;
                color: #0ab6ff;
                background: #fff;
            }
        }
    }
}
</style>