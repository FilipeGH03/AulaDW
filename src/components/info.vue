<template>
    <div>
        <p>Ela utiliza as seguintes tecnologias:</p>
        <p v-if="trabalhar">Não quero trabalhar</p>
        <ul>
            <li>JavaScript</li>
            <li>Vue</li>
            <li>HTML</li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: "Info",
        data() {
            return {
                trabalhar: true,
            }
        }
    }
</script>