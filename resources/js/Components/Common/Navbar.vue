<template>
    <nav class="navbar">
        <div class="container">
            <div class="flex">
                <img style="height: 70px" src="../../../../public/images/tc-shot.png" alt="TC" class="img-fluid">
                <ul class="nav-list flex items-center">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#highlights">Highlights</a></li>
                    <li><a href="#faqs">FAQ's</a></li>
                    <li><a href="#clients">Activities</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </div>
            <div class="buttons">
                <a href="#" class="new-user">Register</a>
                <a href="#" class="login">Login</a>
            </div>
        </div>
    </nav>

</template>

<script setup>
window.onscroll = function() {
    var navbar = document.querySelector('.navbar');
    if (window.scrollY > 50) {
        navbar.classList.add('scrolled');
    } else {
        navbar.classList.remove('scrolled');
    }
};

</script>

<style>
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }

    body {
        font-family: Arial, sans-serif;
        overflow-x: hidden;
        /* background-color: #abbdff; */
    }

    /* Navbar styles */
    .navbar {
        position: fixed;
        top: 0;
        width: 100%;
        background-color: transparent;
        padding: 20px 0;
        z-index: 100;
        transition: background-color 0.3s ease;
        padding: 10px 0 10px 0;
    }

    .navbar.scrolled {
        background-color: #003b0a; /* Color when scrolled */
        box-shadow: 0 4px 2px -2px gray;
    }

    .container {
        width: 100%;
        max-width: 1200px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .nav-list {
        list-style: none;
        margin: 10px 0 10px 0;
    }

    .navbar ul {
        display: flex;
        padding: 0;
        /* margin-top: 0; */
        list-style-type: none;
    }


    .nav-list li {
        margin-right: 20px;
    }

    .nav-list li a {
        text-decoration: none;
        color: rgb(255, 255, 255);
        font-size: 18px;
    }

    .buttons a {
        padding: 10px 20px;
        text-decoration: none;
        color: white;
        border-radius: 4px;
        font-size: 16px;
    }

    .new-user {
        background-color: #777b5e;
        margin-right: 10px;
    }

    .login {
        background-color: #1c6b90;
    }

    /* Section styles for testing scroll behavior */
    .section {
        height: 100vh;
        padding: 100px 20px;
        text-align: center;
        background-color: #f1f1f1;
        margin-top: 80px; /* Adjust to match navbar height */
    }

</style>
