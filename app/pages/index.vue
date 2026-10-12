<script setup lang="ts">
import Carousel from '~/components/ui/carousel/Carousel.vue'
import CarouselContent from '~/components/ui/carousel/CarouselContent.vue'
import CarouselItem from '~/components/ui/carousel/CarouselItem.vue'
import Button from '~/components/ui/button/Button.vue'
import Autoplay from 'embla-carousel-autoplay'


</script>

<template>
    <div class="h-screen">
       <Carousel 
       :plugins="[Autoplay({
      delay: 2000,
    })]"
    :opts="{
        align:'start',
        loop:true,
        dragFree:true
      }"
    >
        <CarouselContent class="w-full" >

          <CarouselItem class="h-svh w-full bg-[url('/images/44570.jpg')]">
            <div class="md:my-20 md:py-20 md:px-20 items-center w-full  bg-black/20">
              <h1 class="text-6xl font-bold text-primary">CENTIC RESEARCH, TEACHING & REFERRAL HOSPITAL</h1>
              <p class="text-white text-2xl font-light py-5">Delivering world-class healthcare, medical education, and innovative research for Kenya and the wider East African region.</p>
              <Button class="bg-green-700 hover:bg-green-800"> Learn More</Button>
            </div>
          </CarouselItem>

          <CarouselItem class="h-svh w-full bg-[url('/images/44570.jpg')]">
            <div class="md:my-20 md:py-20 md:px-20 items-center  bg-black/20">
              <h1 class="text-6xl font-bold text-primary">CENTIC RESEARCH, TEACHING & REFERRAL HOSPITAL</h1>
              <p class="text-white text-2xl font-light py-5">Delivering world-class healthcare, medical education, and innovative research for Kenya and the wider East African region.</p>
              <Button class="bg-green-700 hover:bg-green-800"> Learn More</Button>
            </div>
          </CarouselItem>

          <CarouselItem class="h-svh w-full bg-[url('/images/44570.jpg')]">
            <div class="md:my-20 md:py-20 md:px-20 items-center  bg-black/20">
              <h1 class="text-6xl font-bold text-primary">CENTIC RESEARCH, TEACHING & REFERRAL HOSPITAL</h1>
              <p class="text-white text-2xl font-light py-5">Delivering world-class healthcare, medical education, and innovative research for Kenya and the wider East African region.</p>
              <Button class="bg-green-700 hover:bg-green-800"> Learn More</Button>
            </div>
          </CarouselItem>

        </CarouselContent>
       </Carousel>
    </div>
</template>