<template>
    <div>
        <div class="relative overflow-hidden ">
            <img :src=data.img alt="" class="block w-full h-auto rounded-md">
            <div class="absolute top-0 left-0 right-0 bottom-0 bg-black bg-opacity-40 rounded-md"></div>
            <div class="absolute z-10" style="top: 45%; left: 45%;">
                <img src="/logo-airbnb.png" alt="Logo 1" class="block w-16 h-16">
            </div>
        </div>
        <h5 class="text-xs font-bold mt-2.5" style="color: #914669">
            {{ data.name }}
        </h5>
        <h5 class="text-sm mt-2.5">
            {{ data.desc }}
        </h5>
    </div>
</template>

<script>
export default {
    name: 'ThirdCard',
    props: {
        data: Object
    }
}
</script>