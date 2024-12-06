<template>
    <div class="my-[70px] md:my-[140px]">
    <div class="container mx-auto">
      <div class="lg:grid grid-cols-2 gap-[80px] 2xl:gap-[80px]">
        <div class="relative flex justify-between items-center px-[10px] md:px-0">
          <div class="bg-[#070706] w-[200px] h-[400px] md:w-[400px] md:h-[720px] lg:w-[600px] lg:h-[720px] 2xl:w-[400px] 2xl:h-[720px] rounded-[16px] ml-[50%]"></div>
          <img
            src="../assets/images/team/team9.png"
            alt="team"
            class="w-[90%] md:w-[734px] md:h-[543px] lg:w-[450px] lg:h-[343px] xl:w-[550px] xl:h-[443px] 2xl:w-[650px] 2xl:h-[543px] absolute"
          />
        </div>
        <div class="mt-[20px] px-[10px] md:px-0">
          <p class="text-[#7F27FF] font-[700] text-[15px] md:text-[18px] leading-[26px]">GET IN TOUCH</p>
          <h2 class="my-[8px] md:my-[16px] text-[24px] md:text-[32px] md:leading-[38px] lg:text-[50px] lg:leading-[55px] xl:text-[64px] xl:leading-[72px] font-[700]">
           It’s very easy to contact!
          </h2>
          <div class="md:mt-[30px]">
            <form action="" class="grid gap-[24px]">
                <input type="text" name="name" id="name" placeholder="Your name" class="outline-none border p-[16px] rounded-[4px]">
                <input type="email" name="email" id="email" placeholder="Email address" class="outline-none border p-[16px] rounded-[4px]">
                <input type="text" name="name" id="name" placeholder="Web address" class="outline-none border p-[16px] rounded-[4px]">
                <textarea name="desc" id="desc" cols="30" rows="5" placeholder="Type message" class="outline-none border p-[16px] rounded-[4px]"></textarea>
                <input type="submit" value="SEND MESSAGE NOW" class="p-[16px] bg-[#FF8911] rounded-[4px]">
            </form>
          </div>
        </div>
      </div>
    </div>
    </div>
</template>

<script setup>

</script>

<style lang="scss" scoped>

</style>