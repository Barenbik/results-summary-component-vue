<template>
    <div class="summary-box" :class="`${title.toLowerCase()}-container`">
        <p>
            <i class="fa-solid" :class="`${icon}`"></i>
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
        icon: String
    }
}
</script>

<style>
@import '../assets/main.css';

.reaction-container {
    background-color: hsla(0, 100%, 67%, 0.2);
}

.reaction-container p {
    color: hsl(0, 100%, 67%);
}

.memory-container {
    background-color: hsla(39, 100%, 56%, 0.2);
}

.memory-container p {
    color: hsl(39, 100%, 56%);
}

.verbal-container {
    background-color: hsla(166, 100%, 37%, 0.2);
}

.verbal-container p {
    color: hsl(166, 100%, 37%);
}

.visual-container {
    background-color: hsla(234, 85%, 45%, 0.2);
}

.visual-container p {
    color: hsl(234, 85%, 45%);
}

.summary-box {
    display: flex;
    width: 100%;
    border-radius: 15px;
    flex-direction: row;
    justify-content: space-between;
    margin: 0.625rem 0;
}

.summary-box p {
    margin: 1rem;
}

.summary-score {
    color: hsl(224, 30%, 27%);
    font-weight: bold;
}

.summary-max-score {
    color: hsl(280, 5%, 66%);
}
</style>