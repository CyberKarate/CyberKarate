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

<h3> Our Karate Classes </h3>

<iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfNuQEeVvNqLkIYniCKv20H3jHqI7uXhUxH2l6V5txqk1i2Xw/viewform?embedded=true" width="640" height="1410" frameborder="0" marginheight="0" marginwidth="0">Loading...</iframe>
<iframe width="560" height="315" src="https://www.youtube.com/embed/wGNJDAXyxV4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<head>
<style>
div#test{ border:#000 1px solid; padding:10px 40px 40px 40px; }
</style>
<script>
var pos = 0, test, test_status, question, choice, choices, chA, chB, chC, correct = 0;
var questions = [
    [ "What is the most important thing in a punch?", "Pull back", "Punch", "Stance", "A" ],
	[ "What do you have to do when you pull back?", "Rotate your fist", "Stay low", "Use your hips", "A" ],
	[ "Can you ever be a master at anything?", "Yes", "I do not know", "No", "C", ],
	[ "How often should you practice Karate?", "Once a week", "Everyday", "Twice a week", "B" ]
];
function _(x){
	return document.getElementById(x);
}
function renderQuestion(){
	test = _("test");
	if(pos >= questions.length){
		test.innerHTML = "<h2>You got "+correct+" of "+questions.length+" questions correct</h2>";
		_("test_status").innerHTML = "Test Completed";
		test.innerHTML += "<a href='#'>Re-test</a>";
		test.innerHTML += "<button>Done</button>";
		pos = 0;
		correct = 0;
		return false;
	}
	_("test_status").innerHTML = "Question "+(pos+1)+" of "+questions.length;
	question = questions[pos][0];
	chA = questions[pos][1];
	chB = questions[pos][2];
	chC = questions[pos][3];
	test.innerHTML = "<h3>"+question+"</h3>";
	test.innerHTML += "<input type='radio' name='choices' value='A'> "+chA+"<br>";
	test.innerHTML += "<input type='radio' name='choices' value='B'> "+chB+"<br>";
	test.innerHTML += "<input type='radio' name='choices' value='C'> "+chC+"<br><br>";
	test.innerHTML += "<button onclick='checkAnswer()'>Submit Answer</button>";


}

function checkAnswer(){
	choices = document.getElementsByName("choices");
	for(var i=0; i<choices.length; i++){
		if(choices[i].checked){
			choice = choices[i].value;
		}
	}
	if(choice == questions[pos][4]){
		correct++;
	}
	pos++;
	renderQuestion();
}
window.addEventListener("load", renderQuestion, false);
</script>

<script>
var limit="00:10"
if (document.images){
var parselimit=limit.split(":")
parselimit=parselimit[0]*60+parselimit[1]*1
}
function begintimer(){
	
	</body>
if (!document.images)
return
if (parselimit==1)
window.location="msg.html"
else{ 
parselimit-=1
curmin=Math.floor(parselimit/60)
cursec=parselimit%60
if (curmin!=0)
curtime=curmin+" minutes and "+cursec+" seconds left"
else
curtime=cursec+" seconds left"
window.status=curtime
setTimeout("begintimer()",1000)
}
}

</script>
</head>
<body onLoad="begintimer()">
<h2 id="test_status"></h2>
<div id="test"></div>
</body>



</body>
  
  
  
    

