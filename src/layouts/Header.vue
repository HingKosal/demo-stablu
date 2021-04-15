<template>
    <nav>
        <div class="header_container" id="header">
            <div class="header_content">
                <div class="header_wrapper">
                    <div class="logo">
                        <img :src="logo" alt="logo">
                    </div>
                    <div class="menu">
                        <div class="menu_list">
                            <div class="btn" v-for="(item) in nav_items" :key="item">
                                <span class="child">{{item}} {{index}}</span>
                            </div>
                        </div>
                    </div>
                    <div class="social">
                        <div class="social_list">
                            <div class="icon">
                                <div class="social_icon_child">
                                    <img :src="social_icon" alt="">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
import logo from '../assets/logo.png'
import social_icon from '../assets/social_icon.png'

export default {
    data() {
        return {
            logo: logo,
            social_icon: social_icon,
            nav_items: [
                'Home', 
                'Solutions', 
                'About Us', 
                'Contact Us'
            ]
        };
    }
};
</script>

<style>

    .header_container {
        margin: 0;
        max-height: 150px;
    }

    .header_container .header_content {
        max-width: 1200px;
        margin: auto;
    }

    .header_container .header_content .header_wrapper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        max-width: 1000px;
        margin: auto;
    }

    .header_container .header_content .header_wrapper .logo {
        width: 150px;
    }

    .header_container .header_content .header_wrapper .logo img {
        height: 100%;
        width: 100%;
    }

    .header_container .header_content .header_wrapper .menu .menu_list {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .header_container .header_content .header_wrapper .menu .menu_list .btn {
        color: white;
        font-size: 22px;
        align-items: center;
        margin: 10px 10px;
        padding: 10px 10px;
        cursor: pointer;
    }

    .header_container .header_content .header_wrapper .menu .menu_list .btn .child {
        color: #f1eeee;
        font-size: 20px;
    }

    .header_container .header_content .header_wrapper .menu .menu_list .btn .child:hover {
        /* border-bottom: 3px solid white; */
        transition: all 0.1s;
        color: #fff;
        font: bold;
    }

    .header_container .header_content .header_wrapper .social .social_list .icon {
        width: 60px;
        /* display: flex;
        align-items: center;
        justify-content: space-between; */

    }

    .header_container .header_content .header_wrapper .social .social_list .icon .social_icon_child {
        align-items: center;
        margin:0 5px;
        width: 100%;
    }

    .header_container .header_content .header_wrapper .social .social_list .icon .social_icon_child img {
        width: 100%;
    }
</style>