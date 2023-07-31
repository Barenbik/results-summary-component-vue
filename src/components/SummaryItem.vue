<template>
    <div class="section summary-container">
        <h1 class="summary-title">Summary</h1>
        <summary-box-item v-for="(record, index) in summaryData" :key="index" :title="record.category" :score="record.score"
            :icon="record.icon" />
        <button class="summary-button">Continue</button>
    </div>
</template>

<script>
import SummaryBoxItem from './SummaryBoxItem.vue';
import JsonData from '../data.json';

export default {
    components: {
        SummaryBoxItem
    },
    data() {
        return {
            summaryData: JsonData
        }
    }
}
</script>

<style>
@import '../assets/main.css';

.summary-container {
    display: flex;
    align-items: flex-start;
    width: 85%;
    max-width: 380px;
}

.summary-title {
    color: hsl(224, 30%, 27%);
    margin-top: 1.5rem;
}

.summary-button {
    margin-top: 1rem;
    border-radius: 50px;
    width: 100%;
    padding: 1.5rem;
    background-color: hsl(224, 30%, 27%);
    border: none;
    color: white;
}

@media (min-width: 768px) {
    .summary-container {
        margin: 0 2.5rem;
        width: 50%;
    }
}
</style>