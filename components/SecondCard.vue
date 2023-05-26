<template>
    <div>
        <img :src=data.img alt="" class="w-full rounded-md">

        <div class="flex flex-row items-center justify-between mt-2">
            <div class="flex flex-row items-center">
                <h5 class="text-xs uppercase border border-black rounded-sm p-2">
                    {{ data.name }}
                </h5>
                <h5 class="text-xs text-gray-500 font-light ml-3">
                    {{ data.location }}
                </h5>
            </div>

            <div class="flex flex-row items-center">
                <img src="/star-red.png" alt="" class="mr-1">
                <h5 class="text-xs font-medium">
                    {{ data.rate }}
                </h5>
            </div>
        </div>

        <h5 class="mt-2 text-sm">
            {{ data.desc }}
        </h5>
    </div>
</template>

<script>
export default {
    name: 'SecondCard',
    props: {
        data: Object
    }
}
</script>