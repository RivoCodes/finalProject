<template>
    <div>
        <img :src=data.img alt="" class="rounded-md w-full">
        <h6 class="mt-2 text-xs text-gray-500 font-light">
            {{ data.location }}
        </h6>
        <h5 class="mt-1 text-base text-black font-bold">
            {{ data.name }}
        </h5>
        <h5 class="mt-2 text-sm text-gray-500 font-light">
            {{ data.desc }}
        </h5>
        <div class="flex flex-row items-center mt-2">
            <h5 class="text-sm font-bold" style="color: #008489">
                {{ data.rate }}
            </h5>
            <img src="/star.png" alt="" class="ml-1">
        </div>
    </div>
</template>

<script>
export default {
    name: 'FirstCard',
    props: {
        data: Object
    }
}
</script>