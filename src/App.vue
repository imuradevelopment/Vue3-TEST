<script setup lang="ts">
import DefinePropsComponent from './components/DefinePropsComponent.vue'

</script>

<template id="app">
    <main>
        <ul>
            <li>
                <h2>テンプレート構文</h2>
            </li>
            <DefinePropsComponent msg="テストメッセージ1" />
        </ul>
    </main>
</template>

<style scoped>
    h2 {
        color:var(--vue-green);
    }
</style>
