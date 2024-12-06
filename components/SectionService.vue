<template>
    <div id="service" class="main">
        <div class="container mx-auto px-[10px] xl:px-[10px] 2xl:px-0 py-[70px] md:py-[140px] grid lg:grid-cols-2">
           <div>
                <div class="text-white">
                    <p class="text-[#FF8911] font-[700] text-[15px] md:text-[18px] leading-[26px]">SERVICE</p>
                    <h2 class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]">we Providing Complete Professional IT Services.</h2>
                    <p class="text-white text-[12px] md:text-[16px] md:leading-[20px] lg:text-[15px] lg:leading-[18px] font-[400]">Assertively streamline interactive interfaces after value a infrastructures. Authoritatively fabricate fully tested methodologies before Holistic deliver end-to-end architectures rather sound benefits.</p>
                </div>
                <div class="mt-[64px] px-[10px]">
                    <div v-for="el in data" :key="el.id" class="text-white flex items-center gap-[24px] mt-[40px]">
                        <div class="show bg-[#FF8911] w-[24px] h-[24px]"></div>
                        <div class="w-[90%]">
                            <h3 class="font-[700] text-[18px] md:text-[24px] leading-[28px]">{{el.title}}</h3>
                            <p class="font-[400] text-[12px] md:text-[14px] leading-[23px] mt-[8px] md:mt-[16px]">{{el.desc}}</p>
                        </div>
                    </div>
                </div>
           </div>
           <div class=" md:flex items-center justify-center gap-[24px] mt-[48px] lg:mt-0 px-[20px] md:px-0 lg:ml-[70px] xl:ml-0">
                <div class="grid gap-[24px]">
                    <div class="flex items-center gap-[24px] md:gap-0 md:block lg:w-[230px] xl:w-[300px] xl:h-[350px] 2xl:w-[306px]  2xl:h-[360px] bg-[#ECEEF2] hover:bg-[#FF8911] rounded-[16px] shadow-lg p-4 md:p-6 hover:shadow-xl transition-shadow duration-300">
                        <img src="../assets/images/icons/icon0.png" alt="icon" class="w-[72px] h-[72px] md:w-[72px]">
                        <div class="md:mt-[70px]">
                            <h3 class="text-[24px] leading-[28px] font-[700]">Network solution</h3>
                            <p class="font-[400] text-[#1A1D27CC] text-[16px] leading-[24px]">Assertively streamline interactive interfaces after value-added infrastructures.</p>
                            <div class="py-[16px]">
                                <a href="#" class="text-[#7F27FF]">↗ LEARN MORE</a>
                            </div>
                        </div>
                    </div>
                    <div class="flex items-center gap-[24px] md:gap-0 md:block lg:w-[230px] xl:w-[300px] xl:h-[350px] 2xl:w-[306px]  2xl:h-[360px] bg-[#ECEEF2] hover:bg-[#FF8911] rounded-[16px] shadow-lg p-4 md:p-6 hover:shadow-xl transition-shadow duration-300">
                        <img src="../assets/images/icons/icon1.png" alt="icon" class="w-[72px] h-[72px] md:w-[72px]">
                        <div class="md:mt-[70px]">
                            <h3 class="text-[24px] leading-[28px] font-[700]">Cyber security</h3>
                            <p class="font-[400] text-[#1A1D27CC] text-[16px] leading-[24px]">Assertively streamline interactive interfaces after value-added infrastructures.</p>
                            <div class="py-[16px]">
                                <a href="#" class="text-[#7F27FF]">↗ LEARN MORE</a>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="grid gap-[24px] mt-[24px] md:mt-[58px]">
                    <div class="flex items-center gap-[24px] md:gap-0 md:block lg:w-[230px] xl:w-[300px] xl:h-[350px] 2xl:w-[306px]  2xl:h-[360px] bg-[#ECEEF2] hover:bg-[#FF8911] rounded-[16px] shadow-lg p-4 md:p-6 hover:shadow-xl transition-shadow duration-300">
                        <img src="../assets/images/icons/icon2.png" alt="icon" class="w-[72px] h-[72px] md:w-[72px]">
                        <div class="md:mt-[70px]">
                            <h3 class="text-[24px] leading-[28px] font-[700]">Data analytics</h3>
                            <p class="font-[400] text-[#1A1D27CC] text-[16px] leading-[24px]">Assertively streamline interactive interfaces after value-added infrastructures.</p>
                            <div class="py-[16px]">
                                <a href="#" class="text-[#7F27FF]">↗ LEARN MORE</a>
                            </div>
                        </div>
                    </div>
                     <div class=" md:gap-0 md:block lg:w-[230px] xl:w-[300px] xl:h-[350px] 2xl:w-[306px] 2xl:h-[360px] bg-[#ECEEF2] hover:bg-[#FF8911] rounded-[16px] shadow-lg md:p-6 hover:shadow-xl transition-shadow duration-300 cursor-pointer">
                        <img src="../assets/images/icons/arrow.png" alt="icon" class="w-[72px] h-[72px] md:w-[72px] float-right">
                        <h3 class="text-[24px] leading-[28px] font-[700] mt-[30%] md:mt-[80%] lg:mt-[270px] p-[20px] md:p-0">View all services</h3>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { computed } from 'vue'

    const data = [
        {
            id: 1,
            title: 'Analytical research problem findings',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. ' 
        },
        {
            id: 2,
            title: 'Ensure Quality services',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before.'
        },
        {
            id: 3,
            title: 'Provide in time Delivery',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits.'
        }
    ]

    const card = [
            {
                id: 1,
                icon: 'bx bx-notepad',
                title: 'Network solution',
                desc: ''
            },
            {
                id: 2,
                icon: 'bx bx-pencil',
                title: 'Cyber security',
                desc: "Assertively streamline interactive interfaces after value-added infrastructures."
            },
            {
                id: 3,
                icon: 'bx bx-line-chart',
                title: 'Analyze',
                desc: 'Assertively streamline interactive interfaces after value-added infrastructures.'
            },
            {
                id: 4,
                icon: 'bx bx-rocket',
                title: 'Launch',
                desc: 'Assertively streamline interactive interfaces after value-added infrastructures.'
            }
        ]

        const firstRowCards = computed(() => card.slice(0, 2))
        const secondRowCards = computed(() => card.slice(2, 4))

</script>

<style lang="scss" scoped>
    .main{
            background-image: url(../assets/images/icons/vector.png);   
            background-repeat: no-repeat;
            background-position: center;
            background-size: cover;
        }
    .show{
        box-shadow: -10px -10px 0 white;
    }
</style>