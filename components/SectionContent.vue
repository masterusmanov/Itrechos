<template>
  <div class="my-[70px] md:my-[140px]">
    <div class="container mx-auto">
      <div class="lg:grid grid-cols-2 gap-[80px] 2xl:gap-[80px]">
        <div
          class="relative flex justify-between items-center px-[10px] md:px-0"
        >
          <div
            class="bg-[#070706] w-[200px] h-[400px] md:w-[400px] md:h-[720px] lg:w-[600px] lg:h-[720px] 2xl:w-[400px] 2xl:h-[720px] rounded-[16px] ml-[50%]"
          ></div>
          <img
            src="../assets/images/team/team4.png"
            alt="team"
            class="w-[90%] md:w-[734px] md:h-[543px] lg:w-[450px] lg:h-[343px] xl:w-[550px] xl:h-[443px] 2xl:w-[650px] 2xl:h-[543px] absolute"
          />
        </div>
        <div class="mt-[20px] px-[10px] md:px-0">
          <p
            class="text-[#7F27FF] font-[700] text-[15px] md:text-[18px] leading-[26px]"
          >
            Why choose us
          </p>
          <h2
            class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]"
          >
            Proven Expertise in Complex IT Solutions
          </h2>
          <p
            class="text-[#1A1D27CC] text-[12px] md:text-[16px] md:leading-[20px] lg:text-[15px] lg:leading-[18px] font-[400]"
          >
            Assertively streamline interactive interfaces after value-added
            infrastructures. Authoritatively fabricate fully tested
            methodologies before. Holistic deliver end-to-end architectures
            rather than economically sound benefits. Progressively simplify
            end-to-end paradigms. Assertively streamline interactive interfaces
            after value-added infrastructure.
          </p>
          <div>
            <Accordions />
          </div>
        </div>
      </div>
      <div class="w-[90%] mx-auto mt-[100px]">
        <h5 class="font-[700] text-[32px] leading-[40px]">Ready To Transform Your Business?</h5>
        <div class="grid lg:grid-cols-2 items-center gap-[40px] mt-[56px]">
            <div v-for="el in data" :key="el.id" class="flex md:items-center lg:items-start xl:items-center gap-6">
                <img :src=el.img alt="image" class="w-[60px] h-[60px] md:w-[100px] md:h-full">
                <div>
                    <h6 class="font-[700] text-[18px] md:text-[24px] leading-[28px]">{{el.title}}</h6>
                    <p class="text-[#1A1D27CC] font-[400] text-[12px] md:text-[14px] md:leading-[23px] mt-[8px] md:mt-[16px]">{{el.desc}}</p>
                </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
    import img1 from '../assets/images/cards/card1.png'; 
    import img2 from '../assets/images/cards/card2.png'; 
    import img3 from '../assets/images/cards/card3.png'; 
    import img4 from '../assets/images/cards/card4.png'; 
    const data = [
        {
            id: 1,
            img: img1,
            title: 'Tech Solution',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. '
        },
        {
            id: 2,
            img: img2,
            title: 'Quick Support',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. '
        },
        {
            id: 3,
            img: img3,
            title: 'IT Project Solution',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. '
        },
        {
            id: 4,
            img: img4,
            title: 'Solving IT Challenges',
            desc: 'Assertively streamline interactive interfaces after value-added infrastructures. Authoritatively fabricate fully tested methodologies before. Holistic deliver end sound benefits. '
        }
    ]
</script>

<style lang="scss" scoped></style>
