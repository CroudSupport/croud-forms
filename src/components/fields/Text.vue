<template>
    <div class="ui fluid input" :class="{transparent: transparent}">
        <span v-if="readOnly">{{ value }}</span>
        <input v-else type="text" :placeholder="placeholder" v-model="value">
    </div>
</template>

<script>
    import Input from '../../mixins/Input'

    export default {
        mixins: [
            Input,
        ],
    }
</script>
