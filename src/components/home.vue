<template>
    <div class="flex items-center w-full relative z-1 bg-[#070d1b]">
        <div class="w-full md:w-[50%] flex items-start flex-col justify-center gap-[0.5rem] bg-[#070d1b] md:p-[2rem] p-[1rem] pt-[2rem] mt-[-2rem]">
            <h1 data-aos="fade-up" data-aos-duration="800" data-aos-offset="100" data-aos-easing="ease-in-out" class="text-[#fec544] text-[25px] font-bold">Hello, I am</h1>
            <div data-aos="fade-up" data-aos-duration="1400" data-aos-offset="100" data-aos-easing="ease-in-out" class="md:text-[90px] text-[50px] md:leading-[7rem] leading-[4rem] font-bold text-white w-full">Abdulganiyu Abdulazeez</div>
            <p data-aos="fade-up" data-aos-duration="1600" data-aos-offset="100" data-aos-easing="ease-in-out" class="md:text-[35px] text-[25px] text-gray-500">Website Developer</p>
            <a data-aos="fade-up" data-aos-duration="1700" data-aos-offset="100" data-aos-easing="ease-in-out" href="https://api.whatsapp.com/send?phone=2347010233344" target="_blank" class="bg-[#fec544] px-[4rem] py-[0.8rem] w-fit rounded-[24px] mt-[1rem]">Hire Me</a>
        </div>
        <div class="w-[50%] h-screen bg-[#070d1b] hidden md:flex relative z-1 left-0 items-end anime">
            <div data-aos="fade-right" data-aos-duration="800" data-aos-offset="200" data-aos-easing="ease-in-out" class="w-[50rem] absolute left-[-99%] z-1 flex items-center gap-[2rem] rounded-tl-[45px] rounded-bl-[45px] p-[1rem] border-[1px] border-solid border-gray-700 w-full h-fit bg-[#101624]">
                <a href="https://api.whatsapp.com/send?phone=2347010233344" target="_blank"><div class="fa fa-github cursor-pointer text-white text-[25px] font-bold text-gray-700 rounded-[50%] border-[1px] border-solid border-gray-700 flex items-center justify-center p-[1rem]"></div></a>
                <a href="https://www.linkedin.com/in/abdulazeez-abdulganiyu-072806264" target="_blank"><div class="fa fa-linkedin cursor-pointer text-white text-[25px] font-bold text-gray-700 rounded-[50%] border-[1px] border-solid border-gray-700 flex items-center justify-center p-[1rem]"></div></a>
                <a href="https://www.twitter.com/Abdulaz94349364" target="_blank"><div class="fa fa-twitter cursor-pointer text-white text-[25px] font-bold text-gray-700 rounded-[50%] border-[1px] border-solid border-gray-700 flex items-center justify-center p-[1rem]"></div></a>
                <a href="https://www.instagram.com/abdulganiyu4252/" target="_blank"><div class="fa fa-instagram cursor-pointer text-white text-[25px] font-bold text-gray-700 rounded-[50%] border-[1px] border-solid border-gray-700 flex items-center justify-center p-[1rem]"></div></a>
            </div>
            <img data-aos="fade-left" data-aos-duration="800" data-aos-offset="200" data-aos-easing="ease-in-out" src="../assets/images/blog3-removebg-preview.png" alt="my picture" class="w-full h-full absolute z-2">
        </div>
    </div>
</template>

<style>
    .anime {
        animation-name: anime;
        animation-delay: 2s;
        animation-duration: 5s;
        animation-timing-function: ease;
        animation-iteration-count: infinite;
        animation-direction: alternate;
    }
    @keyframes anime {
        0% {
            top: 0;
            left: 0vw;
        }
        100% {
            top: 0;
            left: 3vw;
        }
    }
</style>