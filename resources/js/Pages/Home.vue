<template>
    <div class="min-h-screens bg-gray-100">
    <Navbar/>
        <div style="padding: 100px 0 0 0" class="first-sec">
            <!-- <BoardHeader/> -->
            <div class="grid grid-cols-12 gap-4">
                <div class="col-span-1 p-4"></div>
                <div class="col-span-10 bg-gray-500 p-4">
                    <BoardHeader/>
                    <div class="grid grid-cols-12 gap-4">
                        <div class="col-span-3 pt-5">
                            <SideBar/>
                        </div>
                        <div class="col-span-9">
                            <MainDisplay/>
                        </div>
                    </div>
                </div>
                <div class="col-span-1 p-4"></div>
            </div>
        </div>
    </div>

    <!-- <Footer/> -->
</template>

<script setup>
import Navbar from '@/Components/Common/Navbar.vue'
import Footer from '@/Components/Common/Footer.vue'
import BoardHeader from '@/Components/Board/Header.vue'
import SideBar from '@/Components/Board/SideBar.vue'
import MainDisplay from '@/Components/Board/MainDisplay.vue'
</script>

<style>
.min-h-screens{
    background-color: rgb(147, 151, 152);
    height: 5000px;
}
</style>
