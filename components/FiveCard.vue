<template>
    <div class="flex my-14">
        <div class="md:flex bg-white w-96 md:mr-20 pr-52 box-border drop-shadow-lg rounded-xl dark:bg-slate-800">
            <img class="w-auto md:w-48 md:h-auto md:rounded rounded-full " :src="data.img" alt="">
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