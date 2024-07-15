<script setup lang="ts">

</script>

<template>
    <aside>
        Sidebar
    </aside>
</template>

<style lang="scss" scoped>
aside {
    display: flex;
    flex-direction: column;
    width: var(--sidebar-width);
    overflow: hidden;
    min-height: 100vh;
    padding: .5rem;

    background-color: var(--darkdark);

    @media (max-width: 768px) {
        position: fixed;
        z-index: 99;
    }
}
</style>