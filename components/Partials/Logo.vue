<template>
    <!-- begin:: Brand -->
    <div class="kt-aside__brand kt-grid__item " id="kt_aside_brand">
        <div class="kt-aside__brand-logo">
            <a href="demo7/index.html">
                <img alt="Logo" :src="image" />
            </a>
        </div>
    </div>

    <!-- end:: Brand -->
</template>
<script>
export default{
    data(){
        return{
            image: '~assets/media/logos/logo-7.png'
        }
    }
}
</script>