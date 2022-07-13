<template>
<form action="">
    <div>
        <InputText />
    </div>
    <div>
        <InputText />
    </div>
    <div>
        <InputSubmit />
    </div>
</form>
</template>

<script>
import InputText from './Form/InputText.vue'
import InputSubmit from './Form/InputSubmit.vue'

export default {
    name: "MyForm",
    components: {
        InputText,
        InputSubmit
    }
}
</script>