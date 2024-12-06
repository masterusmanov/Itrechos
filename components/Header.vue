<template>
    <div class="bg-[#070706] z-100 ">
        <div class="container mx-auto flex items-center justify-between h-[96px] py-[24px]  px-[10px] lg:px-0 xl:px-[10px] 2xl:px-0">
           <h1 class="text-[#FFFFFF] text-[24px] leading-[32px] font-[800]">Itrechos</h1>
           <div class="text-[#FFFFFF] hidden lg:flex items-center justify-between gap-[56px] w-[750px] ">
                <div class="flex items-center gap-[56px]">
                    <a href="#home" class=" text-[16px]">HOME</a>
                    <a href="#service" class=" text-[16px]">SERVICES</a>
                    <a href="#page" class=" text-[16px]">PAGES</a>
                    <a href="#blog" class=" text-[16px]">BLOG</a>
                    <a href="#contact" class=" text-[16px]">CONTACT</a>
                </div>
                <i class='bx bx-phone-call flex items-center  leading-[26px] text-[22px]'> <span class="ml-[6px] font-[700] text-[18px]">+49 30 9846565</span></i>
           </div>
           <i class='bx bx-phone-call hidden md:flex lg:hidden items-center leading-[26px] text-white ml-[300px] text-[16px] font-[700]'> <span class="ml-[6px]">+49 30 9846565</span></i>
           <Menubar class="lg:hidden"/>
        </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>