<template>
    <div class="bg-div pl-5 pb-5 flex flex-row drop-shadow-lg">
        <div class="flex flex-col">
            <div class="ml-2 progress-bar">
                <progress value="100" min="0" max="100" style="visibility:hidden;height:0;width:0;">100%</progress>
            </div>
            <div class="flex items-center justify-center pt-2 text-white text-xs">
                <p>Portugues</p>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="ml-5 progress-bar-2">
                <progress value="100" min="0" max="100" style="visibility:hidden;height:0;width:0;">100%</progress>
            </div>
            <div class="flex items-center justify-center pt-2 text-white text-xs ml-5">
                <p>English</p>
            </div>
        </div>
        <div class="flex flex-col">
            <div class="ml-5 progress-bar-3">
                <progress value="100" min="0" max="100" style="visibility:hidden;height:0;width:0;">100%</progress>
            </div>
            <div class="flex items-center justify-center pt-2 text-white text-xs ml-5">
                <p>Spanish</p>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    props: {
        percentage: {
            type: Number,
            required: true,
        },
        title: {
            type: String
        }
    },
};
</script>
  
<style>
.progress-bar {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background:
        radial-gradient(closest-side, #2b2b35 79%, transparent 80% 100%),
        conic-gradient(#ffc107 100%, #24242f 0);
}

.progress-bar::before {
    content: "100%";
    font-size: small;
    color: white;
}

.progress-bar-2 {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background:
        radial-gradient(closest-side, #2b2b35 79%, transparent 80% 100%),
        conic-gradient(#ffc107 75%, #24242f 0);
}

.progress-bar-2::before {
    content: "75%";
    font-size: small;
    color: white;
}

.progress-bar-3 {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 45px;
    height: 45px;
    border-radius: 50%;
    background:
        radial-gradient(closest-side, #2b2b35 79%, transparent 80% 100%),
        conic-gradient(#ffc107 40%, #24242f 0);
}

.progress-bar-3::before {
    content: "40%";
    font-size: small;
    color: white;
}
</style>
  