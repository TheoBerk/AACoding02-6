# AACoding02-6
<html
 <script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<h1>Gary's Awesome Math Problems</h1>
<div>Timer: <span id="theTime">0</span> Score: <span id="score">0</span></div>
<ol>
  <li>\( 2^3 \) <input data-correct="8"/> </li>
  <li>\( \sqrt[3]{8} \)  <input data-correct="2" /></li>
  <li>\( 8^\frac{1}{3} \) <input data-correct="2"/></li>
  <li>\(   (\frac{-125}{27})^\tfrac{-2}{3} \) <input data-correct="9/25"/></li>
  

</ol>

<CSS>
 .correct{
  background:green;
}

.incorrect{
  background:red;
}

<JS>
 setInterval(upTime,1000);

function upTime(){
  let theTime = Number($("#theTime").text());
  theTime = theTime + 1;
  $("#theTime").text(theTime);
}
$("input").change(onChange);

function onChange(evt){
  let correct = $(this).data("correct");
  let response = $(this).val();
  
  if(correct == response){
    $(this).removeClass('incorrect').addClass("correct");
    let theScore = Number($("#score").text());
    theScore = theScore + 1;
    $("#score").text(theScore);
  } else{
    $(this).removeClass('correct').addClass("incorrect");
  }
}
