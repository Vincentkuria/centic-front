<script setup lang="ts">

</script>

<template>
    <div class="p-10 flex flex-wrap justify-between">
        <div class="h-20">
            <NuxtImg src="/logo.png" class="h-full"/>
        </div>
        <div>
            <h1 class="font-bold flex flex-wrap">Get In Touch</h1>
            <ul>
                <li> <icon name="material-symbols:call-outline" /> +254712345678</li>
                <li> <icon name="material-symbols:location-on-rounded" /> Homa bay County</li>
                <li> <icon name="material-symbols:mark-email-unread-sharp"/> info@centichospital.com</li>
            </ul>
        </div>
        <div>
            <h1 class="font-bold flex flex-wrap p-5" >Socials</h1>
            <div class="flex flex-row gap-5">
                <icon name="meteor-icons:instagram"/>
                <icon name="basil:linkedin-outline"/>
                <icon name="mynaui:brand-facebook"/>
            </div>

        </div>
    </div>
</template>