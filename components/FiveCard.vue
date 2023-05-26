<template>
    <div class="mx-20 my-10">
        <div class="md:flex flex-row bg-white border shadow-lg rounded-xl p-8 md:p-0 dark:bg-slate-800">
            <img class="w-24 h-24 md:w-48 md:h-auto md:rounded rounded-full " :src="data.img" alt="" width="384" height="512">
                <div class="pb-8 md:p-10 text-center md:text-center">
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