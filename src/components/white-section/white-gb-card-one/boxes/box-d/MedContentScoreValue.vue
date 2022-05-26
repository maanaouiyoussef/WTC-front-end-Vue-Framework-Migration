<template>
    <div class="row g-2">
        <div class="col text-center">
            <div class="card m-content-score-box">
                <span style="font-size: 10px">YOUR MEDICAL CONTENT SCORE</span>
                <div id="medical-content-score-value">58.01%</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MedContentScoreValue',
    components: {

    }
}
</script>


<style scoped>
.m-content-score-box {
  font-weight: bold;
  color: white;
  background-image: linear-gradient(to right, #5879d3, #0946ec);
  padding: 10px 18px;
}
</style>