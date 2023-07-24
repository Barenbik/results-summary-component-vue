<template>
    <div class="section result-container">
        <h1 class="lavender-font">Your Result</h1>
        <div class="score-container">
            <div class="score-content">
                <p class="score">76</p>
                <p class="lavender-font">of 100</p>
            </div>
        </div>
        <div class="result-description-container">
            <p class="result-adjective">Great</p>
            <p class="result-description lavender-font">You scored higher than 65% of the people who have taken
                these tests.
            </p>
        </div>
    </div>
</template>

<style>
@import '../assets/main.css';

.result-container {
    align-items: center;
    background: linear-gradient(hsl(252, 100%, 67%), hsl(241, 81%, 54%));
    border-radius: 0 0 35px 35px;
    max-width: 450px;
}

.result-container h1 {
    font-weight: 500;
    padding: 1rem;
}

.lavender-font {
    color: hsl(241, 100%, 89%);
}

.score-container {
    align-items: center;
    background: linear-gradient(hsla(256, 72%, 46%, 1), hsla(241, 72%, 46%, 0));
    border-radius: 50%;
    display: flex;
    height: 150px;
    justify-content: center;
    width: 150px;
}

.score-container p {
    margin: 0;
}

.score-content {
    text-align: center;
}

.score {
    font-size: 3.75rem;
    font-weight: bold;
}

.result-description-container {
    align-items: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    text-align: center;
}

.result-adjective {
    font-size: 24px;
    margin-bottom: 0;
}

.result-description {
    padding-bottom: 1rem;
    width: 60%;
}

@media (min-width: 768px) {
    .result-container {
        border-radius: 35px;
        height: 30rem;
        width: 50%;
    }
}
</style>