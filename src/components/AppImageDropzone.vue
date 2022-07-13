<script setup lang="ts">
import{useBase64, useDropZone} from "@vueuse/core";
import {ref} from "vue";
const dropzoneEl = ref<HTMLElement | null>();
const {} = useDropZone();


function onFileChange(e: any) {
    file.value = any.
    const file = e.target.files[0];
    if (!file)
        console.log(e.target.files);

}
</script>
<template>
<div ref="dropzoneEl"
class="flex m-4"
:class="{border:isOverDropZone,}">


</div>
    <div>AppImageDropzone</div>
    <div class="flex" style="width: 300px; height: 100px; background: #3335">
        <img v-if="url">
        </img>


        <input clase="absolute z-1 left-0 top-0 right-0 left-0 opacity-0" type="file" accept="image/*"
            @input="onFileChange" />
    </div>
    <div class="m-auto opacity-50">Drop a image </div>
    
</template>