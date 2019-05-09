<template>
    <p>
        hello vue {{val}
        <button v-on:click="sendEvent()">5로 변경</button>
    </p>
</template>

<script>
export default {
    name: 'HelloVue',
    props: ['val'],
    methods: {
        sendEvent() {
            this.$emit("change", 5);
        }
    }
}
</script>