<template>
    <form action="">
        <div>
            <InputText></InputText>
            <InputText></InputText>
            <Submit></Submit>
        </div>
    </form>
</template>

<script>


import InputText from './Form/InputText.vue';
import Submit from './Form/Submit.vue';


    export default{
        name: 'Form',
        components:{
            InputText,
            Submit
        }
    }
</script>