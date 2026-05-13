<script setup>
import Button from '../Components/Button.vue';
</script>
<template>
    <section class="section">
        <h2 class="title is-4">Colors</h2>
        <div class="buttons">
            <Button>Default</Button>
            <Button color="primary">Primary</Button>
            <Button color="link">Link</Button>
            <Button color="info">Info</Button>
            <Button color="success">Success</Button>
            <Button color="warning">Warning</Button>
            <Button color="danger">Danger</Button>
            <Button color="dark">Dark</Button>
            <Button color="light">Light</Button>
        </div>

        <h2 class="title is-4">Sizes</h2>
        <div class="buttons">
            <Button color="primary" size="small">Small</Button>
            <Button color="primary" size="normal">Normal</Button>
            <Button color="primary" size="medium">Medium</Button>
            <Button color="primary" size="large">Large</Button>
        </div>

        <h2 class="title is-4">Outlined</h2>
        <div class="buttons">
            <Button color="primary" outlined>Primary</Button>
            <Button color="info" outlined>Info</Button>
            <Button color="success" outlined>Success</Button>
            <Button color="danger" outlined>Danger</Button>
        </div>

        <h2 class="title is-4">Rounded</h2>
        <div class="buttons">
            <Button color="primary" rounded>Primary</Button>
            <Button color="info" rounded>Info</Button>
            <Button color="success" rounded>Success</Button>
            <Button color="danger" rounded>Danger</Button>
        </div>

        <h2 class="title is-4">Loading</h2>
        <div class="buttons">
            <Button color="primary" loading>Loading</Button>
            <Button color="info" loading>Loading</Button>
        </div>

        <h2 class="title is-4">Disabled</h2>
        <div class="buttons">
            <Button color="primary" disabled>Disabled</Button>
            <Button color="danger" disabled>Disabled</Button>
        </div>

        <h2 class="title is-4">Combined</h2>
        <div class="buttons">
            <Button color="success" size="large" rounded outlined>Large Rounded Outlined</Button>
            <Button color="danger" size="small" rounded>Small Rounded</Button>
        </div>
    </section>
</template>
