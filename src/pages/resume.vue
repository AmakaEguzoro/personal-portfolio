<template>
    <div class="row about-me-row">
    <div class="col-md-6">
        <p></p>
    </div>
    <div class="col-md-6 details-about-me">
    <p class="question">My Resume</p>
    <p class="words-about-me">My resume gives an insight to my educational background, age and achievements</p>
    <!-- dont forget to add your resume in google drive -->
    <button type="button" class="btn btn-lg">Download Resume</button>
    </div>
    </div>
</template>
<script>
export default {
    setup() {
        
    },
}
</script>

<style scoped>
.details-about-me {
  padding: 30px;
}

.question {
  font-family: "Comic Sans MS";
  color: #e1c699;
}
.words-about-me {
  font-family: "Garamond"; 
  color: #fff;
  font-size: 20px;
}
.btn{
    background-color: #e1c699;
    color: #000;
    font-family: "Comic Sans MS";
    justify-self: center;
}
</style>