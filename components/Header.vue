<template>
    <div id="mynav">
        <nav :class='"fixed flex flex-row items-center justify-between py-5 px-8 w-full " + this.getBg()'>
            <img src="/Vector.png" class="w-6.5 h-7" alt="">
            <div class="flex item-center space-x-6 py-2 px-3 text-white font-roboto">
                <NuxtLink to="/">Français (FR)</NuxtLink>
                <NuxtLink to="/">EUR €</NuxtLink>
                <NuxtLink to="/">Devenir hôte</NuxtLink>
                <NuxtLink to="/">Créer son expérience</NuxtLink>
                <NuxtLink to="/">Aide</NuxtLink>
                <NuxtLink to="/">Inscription</NuxtLink>
                <NuxtLink to="/">Connexion</NuxtLink>
            </div>
        </nav>
    
        <div class="top-content">
            <img class="md:mx-auto w-full bg-cover" src="/HERO.png" alt="">
                <div class="md:absolute bg-white rounded-md left-20 bottom-28 py-8 px-6" style="max-width: 391px; max-height: 508px;">
                    <h1 class="text-3xl font-medium leading-9">Réservez des hébergements et des activités uniques.</h1>
                    <div class="w-full mt-5">
                        <label class="text-xs w-4 h-3.5 uppercase" for="Où">
                            Où
                        </label>
                        <input type="" class="border w-full h-12 text-gray-700 mt-1 px-4 rounded-sm" placeholder="Partout">
                    </div>
                    <div class="w-full flex flex-row mt-3">
                        <div>
                            <label class="text-xs w-4 h-3.5 uppercase" for="Où">
                                Arrivée
                            </label>
                            <input type="date" class="border w-full h-12 text-gray-700 mt-1 px-4 rounded-sm" placeholder="Partout">
                        </div>
                        <div>
                            <label class="text-xs w-4 h-3.5 uppercase" for="Où">
                                Départ
                            </label>
                            <input type="time" class="border w-full h-12 text-gray-700 mt-1 px-4 rounded-sm " placeholder="Partout">
                        </div>
                    </div>
                    <div class="w-full mt-3">
                        <label class="text-xs w-4 h-3.5 uppercase" for="Où">
                            Voyageurs
                        </label>
                        <input type="" class="border w-full h-12 text-gray-700 mt-1 px-4 rounded-sm" placeholder="Voyageurs">
                    </div>
                    <button class=" rounded-lg bg-red-500 h-12 mt-6 float-right w-40 text-white">
                        Rechercher
                    </button>
                </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Header',
    props: {
        topOfPage: Boolean
    },
    methods: {
        getBg() {
            return this.topOfPage ? "" : "bg-black"
        }
    }
}
</script>