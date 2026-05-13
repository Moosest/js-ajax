<script setup>
let props = defineProps({
    color: {
        type: String,
        validator(value, props) {
            return [
                'white',
                'light',
                'dark',
                'black',
                'text',
                'ghost',
                'primary',
                'link',
                'info',
                'success',
                'warning',
                'danger'
            ].includes(value);
        }
    },
    size: {
        type: String,
        validator(value, props) {
            return [
                'small',
                'normal',
                'medium',
                'large',
            ].includes(value);
        }
    },
    outlined: {
        type: Boolean,
        default: false
    },
    rounded: {
        type: Boolean,
        default: false
    },
    loading: {
        type: Boolean,
        default: false
    },
    disabled: {
        type: Boolean,
        default: false
    }
});

let classes = '';
if (props.color) {
    classes += 'is-' + props.color;
}
if (props.size) {
    classes += ' is-' + props.size;
}
if (props.outlined) {
    classes += ' is-outlined';
}
if (props.rounded) {
    classes += ' is-rounded';
}
if (props.loading) {
    classes += ' is-loading';
}
</script>
<template>
    <button class="button" :class="classes" :disabled="disabled">
        <slot></slot>
    </button>
</template>
