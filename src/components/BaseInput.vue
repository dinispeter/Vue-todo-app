<template>
    <div>
        <input 
            type="text"
            class="input"
            :value="value"
            v-on="listeners"
        />
    </div>
</template>

<script>
export default {
    // props definition
    props: {
        value: {
            type: String,
            default: "",
        }
    },

    computed: {
        listeners() {
            return {
               // Pass all component listeners directly to input 
                ...this.$listeners,
                input: event => this.$emit('input', event.target.value)
            }
        }
    }
}
</script>

<style scoped>
    .input {
        width: 100%;
        padding: 8px 10px;
        border: 2px solid #32485F;
    }
</style>