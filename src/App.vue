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