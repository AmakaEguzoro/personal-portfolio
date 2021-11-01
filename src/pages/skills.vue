<template>
  <div class="row about-me-row">
    <div class="col-md-6">
      <p></p>
    </div>
    <div class="col-md-6 ">
      <p class="question">What Skills do I Possess?</p>
      <div>
          <div class="row programming-skills">
               <p class="col-lg-6">HTML 5</p>
                <p class="col-lg-6 percent">80%</p>
          </div>
         
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          style="width: 80%"
          aria-valuenow="80"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      </div>
     
      <br />
      <div>
          <div class="row programming-skills">
               <p class="col-lg-6">CSS 3</p>
                <p class="col-lg-6 percent">70%</p>
          </div>
         
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          style="width: 70%"
          aria-valuenow="70"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      </div>
      <br />
      <div>
          <div class="row programming-skills">
               <p class="col-lg-6">JavaScript </p>
                <p class="col-lg-6 percent">50%</p>
          </div>
         
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          style="width: 50%"
          aria-valuenow="50"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      </div>
      <br />
      <div>
          <div class="row programming-skills">
               <p class="col-lg-6">TypeScript </p>
                <p class="col-lg-6 percent">70%</p>
          </div>
         
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          style="width: 80%"
          aria-valuenow="80"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      </div>
      <br />
      <div>
          <div class="row programming-skills">
               <p class="col-lg-6">VUE JS </p>
                <p class="col-lg-6 percent">50%</p>
          </div>
         
      <div class="progress">
        <div
          class="progress-bar"
          role="progressbar"
          style="width: 50%"
          aria-valuenow="50"
          aria-valuemin="0"
          aria-valuemax="100"
        ></div>
      </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  setup() {},
};
</script>

<style scoped>

.question {
  font-family: "Comic Sans MS";
  color: #e1c699;
}
.words-about-me {
  font-family: "Garamond";
  color: #fff;
  font-size: 20px;
}
.programming-skills{
    font-family: "Garamond";
  color: #fff;
}
.percent{
    text-align: right;
}
.progress-bar{
    background-color: #e919e9;;
}
</style>
