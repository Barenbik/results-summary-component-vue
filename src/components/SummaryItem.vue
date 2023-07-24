<template>
    <div class="section summary-container">
        <h1 class="summary-title">Summary</h1>
        <summary-box-item title="Reaction" score="80" icon="fa-bolt" />
        <summary-box-item title="Memory" score="92" icon="fa-brain" />
        <summary-box-item title="Verbal" score="61" icon="fa-comment-dots" />
        <summary-box-item title="Visual" score="72" icon="fa-eye" />
        <button class="summary-button">Continue</button>
    </div>
</template>

<script>
import SummaryBoxItem from './SummaryBoxItem.vue';

export default {
    components: {
        SummaryBoxItem
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