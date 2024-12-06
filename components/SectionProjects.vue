<template>
    <div id="page" class="main">
        <div class="container mx-auto py-[70px] md:py-[140px] text-white">
            <div class="px-[10px] md:px-0 md:w-[50%] lg:w-[60%] 2xl:w-[50%]">
                <p class="text-[#FF8911] font-[700] text-[15px] md:text-[18px] leading-[26px]">PROJECTS</p>
                <h2 class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]">Awesome works for our Clients</h2>
                <p class="text-white text-[12px] md:text-[16px] md:leading-[20px] lg:text-[15px] lg:leading-[18px] font-[400]">Assertively streamline interactive interfaces after value a infrastructures. Authoritatively fabricate fully tested methodologies before Holistic deliver end-to-end architectures rather sound benefits.</p>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 items-center gap-[24px] justify-between pt-[56px] px-[10px] md:px-0">
                <div v-for="el in limitedData" :key="el.id" class="box h-[400px]" :style="{backgroundImage: `url(${el.image})`}">
                    <div class="mt-[220px] 2xl:mt-[250px] bg-white rounded-[5px] text-[#070706] mx-auto  px-[24px] py-[20px] w-[75%]">
                        <p class="text-[#7F27FF] font-[500] text-[12px] leading-[16px]">{{el.titul}}</p>
                        <h6 class="font-[700] lg:text-[14px] xl:text-[20px] 2xl:text-[24px] leading-[28px] my-[8px] hover:text-[#FF8911] cursor-pointer">{{el.title}}</h6>
                        <p class="text-[#1A1D27CC] font-[400] leading-[24px]">{{el.desc}}</p>
                    </div>
                </div>
                <div @click="toggleServiceCards" class="h-[400px] bg-[#FF8911] cursor-pointer">
                    <img src="../assets/images/icons/arrow.png" alt="arrow" class="float-right">
                    <h6 class="mt-[350px] font-[700] text-[#070706] text-[24px] leading-[28px] text-center">View all services</h6>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue';

import img1 from '../assets/images/projects/project1.png';
import img2 from '../assets/images/projects/project2.png';
import img3 from '../assets/images/projects/project3.png';
import img4 from '../assets/images/projects/project4.png';
import img5 from '../assets/images/projects/project5.png';
const showServiceCards = ref(false);
    const data = [
        {
            id: 1,
            image: img1,
            titul: 'TECH',
            title: 'Tech Cover Industry',
            desc: 'There are many variations of passages'
        },
        {
            id: 2,
            image: img2,
            titul: 'TECH',
            title: 'Application Integration',
            desc: 'There are many variations of passages'
        },
        {
            id: 3,
            image: img3,
            titul: 'TECH',
            title: 'Database Design',
            desc: 'There are many variations of passages'
        },
        {
            id: 4,
            image: img4,
            titul: 'TECH',
            title: 'Application Integration',
            desc: 'There are many variations of passages'
        },
        {
            id: 5,
            image: img5,
            titul: 'TECH',
            title: 'Database Design',
            desc: 'There are many variations of passages'
        },
        {
            id: 6,
            image: img1,
            titul: 'TECH',
            title: 'Tech Cover Industry',
            desc: 'There are many variations of passages'
        },
        {
            id: 7,
            image: img2,
            titul: 'TECH',
            title: 'Application Integration',
            desc: 'There are many variations of passages'
        },
        {
            id: 8,
            image: img3,
            titul: 'TECH',
            title: 'Database Design',
            desc: 'There are many variations of passages'
        },
        {
            id: 9,
            image: img4,
            titul: 'TECH',
            title: 'Application Integration',
            desc: 'There are many variations of passages'
        },
        {
            id: 10,
            image: img5,
            titul: 'TECH',
            title: 'Database Design',
            desc: 'There are many variations of passages'
        }
    ]

    const toggleServiceCards = () => {
        showServiceCards.value = !showServiceCards.value;
    };

    const limitedData = computed(() =>
    showServiceCards.value ? data : data.slice(0, 5)
    );
</script>

<style lang="scss" scoped>
    .main{
        background-image: url(../assets/images/icons/vector.png);   
         background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
    .box{
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
</style>