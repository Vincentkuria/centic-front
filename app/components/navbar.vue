<script setup lang="ts">
import NavigationMenu from './ui/navigation-menu/NavigationMenu.vue'
import NavigationMenuList from './ui/navigation-menu/NavigationMenuList.vue'
import NavigationMenuItem from './ui/navigation-menu/NavigationMenuItem.vue'
import NavigationMenuTrigger from './ui/navigation-menu/NavigationMenuTrigger.vue'
import NavigationMenuContent from './ui/navigation-menu/NavigationMenuContent.vue'
import NavigationMenuLink from './ui/navigation-menu/NavigationMenuLink.vue'


</script>

<template>
    <div>
        <div class="p-2 mx-5 hidden md:mx-20 md:flex flex-col md:flex-row justify-around border-b border-b-gray-400">
            <span>Hotline and general info <span class="px-2 rounded-full text-gray-700 bg-gray-300">0712345678</span> </span>
            <NuxtLink to="mailto:info@centichospital.com"> <span>info@centichospital.com</span></NuxtLink>
            <span> <icon name="material-symbols:location-on-rounded" /> Homa bay County</span>
        </div>
        <div class="mx-10 p-2 flex flex-row justify-between items-center" >
            <div class="h-16">
                <NuxtImg src="/logo.png" class="h-full" />
            </div>

            <div class="">
                <NavigationMenu>
                    <NavigationMenuList>

                        <NavigationMenuItem>
                            <NavigationMenuLink as-child>
                                <NuxtLink to="/">Home</NuxtLink>
                            </NavigationMenuLink>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuTrigger>About Us</NavigationMenuTrigger>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuTrigger>Services</NavigationMenuTrigger>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuTrigger>Careers</NavigationMenuTrigger>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuTrigger>Contact Us</NavigationMenuTrigger>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuTrigger>Media Center</NavigationMenuTrigger>
                        </NavigationMenuItem>

                        <NavigationMenuItem>
                            <NavigationMenuLink>
                                <NuxtLink to="/donate">Donate</NuxtLink>
                            </NavigationMenuLink>
                        </NavigationMenuItem>

                    </NavigationMenuList>
                </NavigationMenu>
            </div>
        </div>
    </div>
</template>