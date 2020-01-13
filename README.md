# AACoding02-6
Second day of coding in gary anderson's advanced algebra class
Hello World
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="apple-mobile-web-app-title" content="CodePen">
<title>AACoding02-6</title>
</head>
<body translate="no">
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<h1>Gary's Awesome Math Problems</h1>
<ol>
<li>\( 2^3 \)</li>
<li>\( \sqrt[3]{8} \)</li>
<li>\( 8^\frac{1}{3} \)
</ol>
</body>
</html>
.correct{
  background:green;
}

.incorrect{
  background:red;
}
$("input").change(onChange);
function onChange(evt){
  let correct = $(this).data("correct");
  let response = $(this).val();
  
  if(correct == response){
    $(this).removeClass('incorrect').addClass("correct");
  } else{
    $(this).removeClass('correct').addClass("incorrect");
  }
}
