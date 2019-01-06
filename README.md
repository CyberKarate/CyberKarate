<html>
<head>
<title> JS guessing game </title>
<script type="text/javascript">
var ranNum;
function playGame ( ) {
  var answer;
  var fnd = false;
  var cnt = 10;
  while ((cnt > 0) && (fnd == false)) {
    answer = prompt("Guess a number between 1 and 50!");
    if (answer > ranNum) { alert("Guess lower!"); }
    if (answer < ranNum) { alert("Guess higher!!"); }
    if (answer == ranNum) { alert("Correct!"); fnd = true; }
    cnt--;
  }
  if (!fnd) { alert('Too bad, you lose ... The number was '+ranNum); }
  return fnd;
}
function generateRandomNumber() {
  ranNum = Math.floor(Math.random()*50)+1;
}
window.onload = function() { generateRandomNumber(); }
</script>
</head>
<body>
<strong> Guess a random number </strong>
<input type="button" value="Play game" onclick="playGame()"> 
<input type="button" value="New game" onclick="generateRandomNumber()"> 
</body>
</html>
<body>
<h1> Welcome to Cyber Martial Arts Dojo </h1>
  
  <img src="CyberKarateDojo.PNG">

<p> Welcome to Cyber Martial Arts. Our main goal is to have a <Bold> FREE </Bold> online karate dojo for people who can't afford it. </p>

<h2> Please watch the video below for more information. </h2> 

<iframe width="560" height="315" src="https://www.youtube.com/embed/JidnqqwSkK8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!--
<script type="text/javascript" src="//downloads.mailchimp.com/js/signup-forms/popup/unique-methods/embed.js" data-dojo-config="usePlainJson: true, isDebug: false"></script><script type="text/javascript">window.dojoRequire(["mojo/signup-forms/Loader"], function(L) { L.start({"baseUrl":"mc.us7.list-manage.com","uuid":"208c9cc9c169789616ad68872","lid":"2561fe75da","uniqueMethods":true}) })</script>
<script>(function(t,e,s,n){var o,a,c;t.SMCX=t.SMCX||[],e.getElementById(n)||(o=e.getElementsByTagName(s),a=o[o.length-1],c=e.createElement(s),c.type="text/javascript",c.async=!0,c.id=n,c.src=["https:"===location.protocol?"https://":"http://","widget.surveymonkey.com/collect/website/js/tRaiETqnLgj758hTBazgdxH9NlI1a7W911VCIbYgCRUIX_2Bkt5hcyBomZhqLmFhhJ.js"].join(""),a.parentNode.insertBefore(c,a))})(window,document,"script","smcx-sdk");</script>
-->
<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfNuQEeVvNqLkIYniCKv20H3jHqI7uXhUxH2l6V5txqk1i2Xw/viewform?embedded=true" width="640" height="1410" frameborder="0" marginheight="0" marginwidth="0">Loading...</iframe>


  </body>
  
  
  
    

