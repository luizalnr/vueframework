<template>
    <header class="Header">
        <h1 class="title"><slot name="title" /></h1>

        <div class="description"><slot name="description" /></div>

        <div class="content"><slot /></div>
        
    </header>
</template>




<script>
export default {
     
}
</script>




<style>
    .Header{
        background: #000;
        color: #fff;
    }
</style>
