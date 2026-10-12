<script setup lang="ts">
import Footer from '~/components/footer.vue';
import Navbar from '~/components/navbar.vue';


</script>

<template>
    <div>
        <div>
            <Navbar/>
        </div>
        <div>
            <slot/>
        </div>
        <div>
            <Footer/>
        </div>
    </div>
</template>