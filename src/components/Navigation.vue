<template>
    <!--
3 - Navbar with brand center, links on left and right that all collapse into the vertical mobile
    menu
-->
<nav class="navbar navbar-dark navbar-expand-md bg-success justify-content-between">
    <div class="container-fluid">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target=".dual-nav">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="navbar-collapse collapse dual-nav w-50 order-1 order-md-0">
            <ul class="navbar-nav">
                <li class="nav-item active">
                    <a class="nav-link pl-0" href="#">Home <span class="sr-only">Home</span></a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="//codeply.com">Codeply</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                </li>
            </ul>
        </div>
        <a href="/" class="navbar-brand mx-auto d-block text-center order-0 order-md-1 w-25">
            <img alt="Adellis Corporation" src="../assets/logo_small.png">
        </a>
        <div class="navbar-collapse collapse dual-nav w-50 order-2">
            <ul class="nav navbar-nav ml-auto">
                <li class="nav-item"><a class="nav-link" href=""><i class="fa fa-twitter"></i></a></li>
                <li class="nav-item"><a class="nav-link" href=""><i class="fa fa-github"></i></a></li>
            </ul>
        </div>
    </div>
</nav>
</template>
