<template>
    <div class="flex mx-20 my-10">
        <div class="md:flex bg-white border shadow-lg rounded-xl dark:bg-slate-800">
            <img class="w-auto h-24 md:w-48 md:h-auto md:rounded rounded-full " :src="data.img" alt="">
                <div class="flex-nowrap pb-8 md:p-10 text-center md:text-center">
                    <div>
                        <p class="text-lg font-medium">
                            {{ data.name }}
                        </p>
                    </div>
                </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FiveCard',
    props: {
        data: Object
    }
}
</script>