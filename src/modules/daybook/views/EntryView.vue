<template>
    <div class="entry-title d-flex justify-content-between p-2">
        
        <div>
            <span class="text-sucess fs-3 fw-bold">17</span>
            <span class="mx-1 fs-3">Julio</span>
            <span class="mx-2 fs-4 fw-light">2023, Lunes</span>
        </div>

        <div>
            <button class="btn btn-danger mx-2">
                Borrar
                <i class="fa fa-trash-alt"></i>
            </button>
            <button class="btn btn-primary">
                Subir foto
                <i class="fa fa-upload"></i>
            </button>
        </div>

    </div>
    
    <hr>
    <div class="d-flex flex-column px-3 h-75">
        <textarea 
            placeholder="¿Qué sucedió hoy?">
        </textarea>
    </div>
    <MyFab 
        icon="fa-save"/>
    <img 
        src="https://www.adobe.com/es/express/feature/image/convert/jpg-to-png/media_1b0ad89a4a5ad233f5708e21b5998d6638cb07929.png" 
        alt="entry-picture"
        class="img-thumbnail">
</template>
https://www.adobe.com/es/express/feature/image/convert/jpg-to-png/media_1b0ad89a4a5ad233f5708e21b5998d6638cb07929.png
<script>
import { defineAsyncComponent } from 'vue'

export default {
    components:{
        MyFab: defineAsyncComponent(() => import('../components/MyFab.vue'))
    }
}
</script>

<style lang="scss" scoped>
textarea {
    font-size: 20px;
    border: none;
    height: 100%;

    &:focus {
        outline: none;
    }
}

img{
    width: 200px;
    position: fixed;
    bottom: 150px;
    right: 20px;
    box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2 )
}
</style>