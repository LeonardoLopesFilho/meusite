<template>
    <div class="bg-div pl-5 pb-5 drop-shadow-lg">
        <div class="flex flex-row">
            <div class="mb-1 text-xs font-normal dark:text-white w-5">{{ this.linguagem }}</div>
            <div class="mb-1 text-xs font-normal  dark:text-white pl-36"> {{`${porcentagem}%`}}</div>
        </div>
        <div class="w-48 bg-yellow-300 rounded-full h-1 mb-4 dark:bg-gray-700">
            <div class="bg-gray-600 h-1 rounded-full dark:bg-yellow-500" :style="{ width: `${porcentagem}%` }"></div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        porcentagem:Number,
        linguagem:String
    }
}
</script>

<style></style>