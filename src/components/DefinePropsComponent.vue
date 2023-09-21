<template>
    <div class="col">
        <div>
            <div>
                データバインディングで最も基本の形式は、「マスタッシュ構文」(二重中括弧) によるテキスト展開です
            </div>
            <a href="https://ja.vuejs.org/guide/essentials/template-syntax.html#text-interpolation">
                テキスト展開
            </a>
        </div>
        <div>
            {{ $options.__name }}のテスト：
            <span class="test">{{ msg }}</span>
        </div>
    </div>
</template>

<script setup lang="ts">

defineProps<{
    msg: string
}>()

</script>

<style scoped>
.col {
    display: grid;
    grid-template-columns: 2fr 1fr;
}

.col > div:first-child {
    margin: 0 20px 0 0;
    border-right: dashed 1px var(--vue-green);
}

.test {
    color: var(--vue-green);
}
</style>