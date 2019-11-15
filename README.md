# SayCode
## SayCode - say what you want the code to do

This programming language aims to allow someone who does not know how to code to generate code in the best-practice programming language by using a natural sentence like command and indentation for a better coder user experience.

This also aims tocombine the best parts of all languages it supports and remove the time spent worrying about syntax, missing brackets and not remembering function, method or names of properties of a library by minimising these and just "saying" what you want to get done.

It allows you to create syntax for other programming languages such as HTML, CSS, JavaScript and Python by having operations running in the relevant languages based on what is the best-practice for that operation and the current situation.

The determining factor of what language to use is checked on-code-compile and generates the code based on triggers and checks. This also allows the code to use all existing pre-written libraries without edits.

The language definitions are written in Python - some examples below.

In short - the language allows you to generate code like this:

```
<!DOCTYPE html>
<html>
<link rel="stylesheet" href="/style.css">
<script src="/javascripts/my.js"></script>
<body>
<div class="className" id="idName">
<h1 class="bootstrap-heading">My First Heading</h1>
<p id="paragrpahID">My first paragraph.</p>
</div>
</body>
</html>
```

by writing code that you can say with a lot less formatting and syntax like this:

```
html
style
	from /style.css

script
	from /javascripts/my.js
	
body
	div 
	class className 
	id idName
		h1 
		class bootstrap-heading
		content(My First Heading 123)
		
		p
		id paragraphID
		content(My first paragraph.)
		
end body
end html
```

but also allow you to do operations and use variables that are natural - things like these:

```
<div class="container">
  <div class="hello">Hello</div>
  <div class="goodbye">Goodbye</div>
</div>

<script src="/jQuery.js"></script>
<script>
$( ".hello" ).remove();
</script>
```
now becomes

```
div
class container
	div 
	class hello
	content(Hello)
	
  	div 
	class goodbye
	content(Goodbye)

remove div.class="hello"
```

