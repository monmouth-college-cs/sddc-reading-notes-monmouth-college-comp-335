<!DOCTYPE html>
<html>
<head>
<title>Notes</title>

<script>
function setClassDisplay(type, checked) {
  var effect = (checked) ? "block":"none"; 
  var x = document.getElementsByClassName(type);
  for (var i = 0; i < x.length; i++) {
    x[i].style.display = effect;
  }
}
</script>
</head>
<body>

<pre>
<a href="#1">1: Chapter 1</a>
   <a href="#1.1">1.1: Title One</a>
   <a href="#1.2">1.2: Title Two</a>
</pre>

Display:<br>
<input type="checkbox" onclick="setClassDisplay('summary',this.checked)" checked>Summaries<br>
<input type="checkbox" onclick="setClassDisplay('questions',this.checked)" checked>Questions<br>
<input type="checkbox" onclick="setClassDisplay('references',this.checked)" checked>References<br>

<h1 id="1">Chapter 1</h1>

<h2 id="1.1">1.1: Title One</h2>
<span class="summary">1.1 summary<br><br><br><br><br><br><br><br></span><br>
<span class="questions">1.1 questions<br><br><br><br><br><br><br><br></span><br>
<span class="references">1.1 references<br><br><br><br><br><br><br><br></span><br>
<h2 id="1.2">1.2: Title Two</h2>
<span class="summary">1.2 summary<br><br><br><br><br><br><br><br></span><br>
<span class="questions">1.2 questions<br><br><br><br><br><br><br><br></span><br>
<span class="references">1.2 references<br><br><br><br><br><br><br><br></span><br>

</body>
</html>
