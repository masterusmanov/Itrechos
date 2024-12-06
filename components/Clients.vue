<template>
   <div class="gallery-container">
    <div class="gallery">
        <div v-for="(el, index) in images" :key="index" class="w-[357px] h-[285px] bg-white p-[32px]">
            <div class="text-white flex gap-[2px]">
                <i class='bx bxs-star bg-[#FF8911] p-1' ></i>
                <i class='bx bxs-star bg-[#FF8911] p-1' ></i>
                <i class='bx bxs-star bg-[#FF8911] p-1' ></i>
                <i class='bx bxs-star bg-[#FF8911] p-1' ></i>
            </div>
            <p class="mt-[12px] font-[400] leading-[24px] text-[#1A1D27CC]">{{el.desc}}</p>
            <div class="flex items-center gap-[8px] mt-[12px] ">
                <img :src=el.image alt="image" class="w-[25%] py-[15px]">
                <div>
                    <h6 class="font-[700] text-[18px] leading-[26px]">{{el.name}}</h6>
                    <p class="mt-[12px] font-[400] leading-[24px] text-[#1A1D27CC]">{{el.level}}</p>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<script setup>
    import avatar from "../assets/images/team/avatar.png";
    
    const images = [
        {
            id: 1,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 2,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 3,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 4,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 5,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 6,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 7,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 8,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 9,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 10,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 1,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 2,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 3,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 4,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 5,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 6,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 7,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 8,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 9,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        },
        {
            id: 10,
            image: avatar,
            desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut quisque amet habitant integer pretium hendrerit enim. Lobortis sed phasellus auctor',
            name: 'Paula Brooks',
            level: 'Business Analyst'
        }
    ];
</script>


<style lang="scss" scoped>
    .gallery-container {
        /* width: 100%; */
        overflow: hidden;
        position: relative;
    }

    .gallery {
        display: flex;
        animation: scroll 25s linear infinite;
        gap: 20px;
        width: max-content;
    }

    .gallery img {
        /* width: 200px; */
        height: 100px;
        margin-right: 10px;
    }

    @keyframes scroll {
        0% {
            transform: translateX(0);
        }

        100% {
            transform: translateX(-50%);
        }
    }

    .gallery-container:hover .gallery {
        animation-play-state: paused;
    }
</style>