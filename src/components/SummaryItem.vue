<template>
    <div class="section summary-container">
        <h1>Summary</h1>
        <summary-box-item title="Reaction" score="80" />
        <summary-box-item title="Memory" score="92" />
        <summary-box-item title="Verbal" score="61" />
        <summary-box-item title="Visual" score="72" />
        <button>Continue</button>
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