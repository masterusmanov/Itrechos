<template>
    <div id="blog" class="bg-[#070706] text-white py-[70px] md:py-[140px]">
        <div class="container mx-auto px-[10px] md:px-0">
            <p class="text-[#7F27FF] font-[700] text-[15px] md:text-[18px] leading-[26px]">OUR LATEST BLOG</p>
            <h2 class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]" >
            Our latest experience
            </h2>
            <p class="font-[400] leading-[24px] mt-[8px]">Assertively streamline interactive interfaces after value a infrastructures. Authoritatively fabricate fully <br> tested methodologies before Holistic deliver end-to-end architectures rather sound benefits.</p>
            <p @click="toggleServiceCards" class="text-end text-[#FF8911] font-[500] leading-[23px] cursor-pointer">↗ VIEW ALL</p>
            <div class="grid grid-cols-1 md:grid-cols-3 items-center gap-[24px] my-[28px] md:my-[56px]">
                <div v-for="el in limitedData" :key="el.id" class="" >
                    <img :src=el.image alt="">
                    <div class="mt-[32px]">
                        <p class="font-[400] leading-[24px] text-[#FF8911] ">{{el.time}}</p>
                        <h6 class="font-[700] text-[22px] leading-[28px] mt-[8px] mb-[16px] ">{{el.title}}</h6>
                        <p class="font-[400] leading-[24px] text-white ">{{el.desc}}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';

    import blog1 from '../assets/images/blogs/blog1.png';
    import blog2 from '../assets/images/blogs/blog2.png';
    import blog3 from '../assets/images/blogs/blog3.png';
    const showServiceCards = ref(false);
    const data = [
        {
            id: 1,
            image: blog1,
            time: 'November 21, 2022-Tom Black',
            title: 'Plan Your Project with Your Software',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        },
        {
            id: 2,
            image: blog2,
            time: 'November 21, 2022-Tom Black',
            title: 'You have a Great Business Idea?',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        },
        {
            id: 3,
            image: blog3,
            time: 'November 21, 2022-Tom Black',
            title: 'Building Data Analytics Software',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        },
        {
            id: 4,
            image: blog1,
            time: 'November 21, 2022-Tom Black',
            title: 'Plan Your Project with Your Software',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        },
        {
            id: 5,
            image: blog2,
            time: 'November 21, 2022-Tom Black',
            title: 'You have a Great Business Idea?',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        },
        {
            id: 6,
            image: blog3,
            time: 'November 21, 2022-Tom Black',
            title: 'Building Data Analytics Software',
            desc: 'It is a time tracking solution that helps employees track hours across multiple tasks and projects  software.'
        }
        
    ]

     const toggleServiceCards = () => {
        showServiceCards.value = !showServiceCards.value;
    };

    const limitedData = computed(() =>
    showServiceCards.value ? data : data.slice(0, 3)
    );
</script>

<style lang="scss" scoped>
    .box{
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
</style>