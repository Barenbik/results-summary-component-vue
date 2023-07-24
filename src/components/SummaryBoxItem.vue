<template>
    <div class="reaction-container summary-box">
        <p>
            <i class="fa-solid fa-bolt"></i>
            {{ title }}
        </p>
        <p>
            <span class="summary-score">{{ score }}</span>
            <span class="summary-max-score"> / 100</span>
        </p>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        score: Number,
    }
}
</script>