<template>
    <div class="my-[70px] md:my-[140px]">
        <div class="container mx-auto px-[10px] md:px-0">
            <p class="text-[#7F27FF] font-[700] text-[15px] md:text-[18px] leading-[26px]">OUR TEAM</p>
            <h2 class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]" >
            Our Professional <br> Team member
            </h2>
            <p @click="toggleServiceCards" class="text-end text-[#FF8911] font-[500] leading-[23px] cursor-pointer">↗ VIEW ALL</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 items-center gap-[24px] my-[28px] md:my-[56px]">
                <div v-for="el in limitedData" :key="el.id" class="" >
                    <div class="box h-[512px] rounded-[8px]" :style="{backgroundImage: `url(${el.image})`}">
                        <div class="flex gap-[12px] pt-[450px] pl-[20px]">
                            <i class='bx bxl-facebook bg-[#FF8911] rounded-full p-[10px]'></i>
                            <i class='bx bxl-instagram bg-[#FF8911] rounded-full p-[10px]' ></i>
                            <i class='bx bxl-twitter bg-[#FF8911] rounded-full p-[10px]'></i>
                        </div>
                    </div>
                    <h6 class="font-[700] text-[22px] leading-[28px] mt-[32px]">{{el.title}}</h6>
                    <p class="font-[400] leading-[24px] text-[#1A1D27CC] mt-[8px]">{{el.desc}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';

    import team5 from '../assets/images/team/team5.png';
    import team6 from '../assets/images/team/team6.png';
    import team7 from '../assets/images/team/team7.png';
    import team8 from '../assets/images/team/team8.png';
    const showServiceCards = ref(false);
    const data = [
        {
            id: 1,
            image: team5,
            title: 'Eleanor Pena',
            desc: 'Senior Developer'
        },
        {
            id: 2,
            image: team6,
            title: 'Application Integration',
            desc: 'Senior Developer'
        },
        {
            id: 3,
            image: team7,
            title: 'Database Design',
            desc: 'Senior Developer'
        },
        {
            id: 4,
            image: team8,
            title: 'Application Integration',
            desc: 'Senior Developer'
        },
        {
            id: 5,
            image: team5,
            title: 'Tech Cover Industry',
            desc: 'Senior Developer'
        },
        {
            id: 6,
            image: team6,
            title: 'Application Integration',
            desc: 'Senior Developer'
        },
        {
            id: 7,
            image: team7,
            title: 'Database Design',
            desc: 'Senior Developer'
        },
        {
            id: 8,
            image: team8,
            title: 'Application Integration',
            desc: 'Senior Developer'
        }
        
    ]

     const toggleServiceCards = () => {
        showServiceCards.value = !showServiceCards.value;
    };

    const limitedData = computed(() =>
    showServiceCards.value ? data : data.slice(0, 4)
    );
</script>

<style lang="scss" scoped>
    .box{
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
</style>