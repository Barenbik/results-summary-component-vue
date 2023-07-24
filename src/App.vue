<template>
    <div class="content">
        <result-item />
        <summary-item />
    </div>
</template>

<script>
import ResultItem from './components/ResultItem.vue';
import SummaryItem from './components/SummaryItem.vue'

export default {
    components: {
        ResultItem,
        SummaryItem
    }
}
</script>

<style>
@import '../src/assets/main.css';

.content {
    align-items: stretch;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    min-width: 375px;
}

@media (min-width: 768px) {
    .content {
        flex-wrap: nowrap;
        max-width: 800px;
        margin: auto;
        align-items: center;
        box-shadow: 0 4px 20px 4px hsla(241, 72%, 46%, 0.2);
        border-radius: 35px;
    }
}
</style>