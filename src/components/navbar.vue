<template>
    <nav class="w-full bg-[#070d1b] md:p-[1rem] p-[1rem] py-0 md:py-xl flex justify-between border-b-[1px] border-b-solid border-b-gray-700 relative top-[0rem] z-[9]" :class="window==offset ? 'sticky top-[0] z-2' : 'relative'">
        <!-- logo -->
        <div class="flex items-center gap-[0.5rem]">
            <div class="rounded-[50%] border-[3px] border-solid border-[#fec544] w-[4rem] h-[4rem] p-[0.6rem] overflow-hidden flex items-center justify-center">
                <img class="w-full h-full" src="../assets/images/portfolio Logo.svg" alt="">
            </div>
            <h1 class="text-[40px] text-white"><b><span class="text-[#fec544]">A</span>bdulazeez</b></h1>
        </div>
        <!-- nav-links hidden md:flex items-center gap-[2rem]    :class=" !menu ? 'left-0' : 'left-[-700px]'" @click="back"-->
        <div v-if="conditioning = !conditioning" class="bg-[#070d1b] md:flex flex md:flex-row flex-col md:items-center items-left md:border-none border-b-solid border-b-[1px] border-gray-700 max-[768px]:gap-[1rem] text-white gap-[2rem] top-[4rem] z-50 absolute md:static p-[2rem] md:p-0 flex-col md:flex-row w-full md:w-fit transition-left duration-2000" :class=" !menu ? 'left-0' : 'left-[-700px]'">
            <div><a class="hover:text-[#fec544]" href="#" :class="!condition ? 'text-[#fec544]' : 'text-white'" @click="change">HOME</a></div>
            <div><a class="hover:text-[#fec544]" href="#" :class="!condition1 ? 'text-[#fec544]' : 'text-white'" @click="change1">ABOUT</a></div>
            <div><a class="hover:text-[#fec544]" href="#" :class="!condition2 ? 'text-[#fec544]' : 'text-white'" @click="change2">SKILL</a></div>
            <div><a class="hover:text-[#fec544]" href="#" :class="!condition3 ? 'text-[#fec544]' : 'text-white'" @click="change3">RESUME</a></div>
            <div class="flex gap-[1rem] md:gap-[2rem] items-center w-full">
                <a class="hover:text-[#fec544]" href="#" :class="!condition4 ? 'text-[#fec544]' : 'text-white'" @click="change4">CONTACT</a>
                <p  href="#">|</p>
                <div class="flex items-center gap-[1rem] w-full">
                    <div class="fa fa-phone"></div>
                    <p class="text-[#fec544] p-0 w-full text-[15px]">+234 7010233344</p>
                </div>
            </div>
        </div>
        <!-- menu -->
        <div class="items-center md:hidden  flex">
            <img v-if="determine" @click="determinant" class="w-[1.5rem] h-[1.5rem]" src="../assets/images/icon-hamburger.svg" alt="">
            <img v-else @click="determinant" src="../assets/images/icon-close.svg" alt="">
        </div>

    </nav>
</template>
<script>
import { defineComponent } from 'vue';
export default defineComponent ({
    data() {
        return {
            condition: false,
            condition1: true,
            condition2: true,
            condition3: true,
            condition4: true,
            determine: true,
            conditioning: true,
            menu: true,
            container:document.querySelector('stickyNav')
        }
    },
    methods: {
        change() {
            this.condition = false
            this.condition1 = true
            this.condition2 = true
            this.condition3 = true
            this.condition4 = true
        },
        change1() {
            this.condition = true
            this.condition1 = false
            this.condition2 = true
            this.condition3 = true
            this.condition4 = true
        },
         change2() {
            this.condition = true
            this.condition1 = true
            this.condition2 = false
            this.condition3 = true
            this.condition4 = true
        },
        change3() {
            this.condition = true
            this.condition1 = true
            this.condition2 = true
            this.condition3 = false
            this.condition4 = true
        },
        change4() {
            this.condition = true
            this.condition1 = true
            this.condition2 = true
            this.condition3 = true
            this.condition4 = false
        },
        determinant() {
            this.determine = !this.determine,
            this.conditioning = !this.conditioning
            this.menu = !this.menu
        }

    }
})
</script>
<!-- for other backgroundS: #0a101e -->
<!-- for home bg: #070d1b -->
<!-- for text background beside header: #101624 -->
<!-- for deep yellow: #fec544 -->
<!-- a bit light yellow: #FFC848 -->