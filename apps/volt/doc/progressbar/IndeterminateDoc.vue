<template>
    <DocSectionText v-bind="$attrs">
        <p>For progresses with no value to track, set the <i>mode</i> property to <i>indeterminate</i>.</p>
    </DocSectionText>
    <div class="card">
        <ProgressBar mode="indeterminate" style="height: 6px"></ProgressBar>
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import ProgressBar from '@/volt/ProgressBar.vue';
import { ref } from 'vue';

const code = ref(`
<template>
    <div class="card">
        <ProgressBar mode="indeterminate" style="height: 6px"></ProgressBar>
    </div>
</template>

<script setup lang="ts">
import ProgressBar from '@/volt/ProgressBar.vue';
<\/script>
`);
</script>
