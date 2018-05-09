# HTML
## Table
```
<table border="1">
	<thead>
		<tr>
			<th>Image</th>
			<th>Name</th>
			<th>Type</th>
			<th>Evolves Into</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td><img src="http://img4.wikia.nocookie.net/__cb20140328190757/pokemon/images/thumb/2/21/001Bulbasaur.png/200px-001Bulbasaur.png"></td>
			<td>Bulbasaur</td>
			<td>Grass/Poison</td>
			<td><a href="http://pokemon.wikia.com/wiki/Ivysaur">Ivysaur</a></td>
		</tr>
		<tr>
			<td><img src="http://img4.wikia.nocookie.net/__cb20140724195345/pokemon/images/thumb/7/73/004Charmander.png/200px-004Charmander.png"></td>
			<td>Charmander</td>
			<td>Fire</td>
			<td><a href="http://pokemon.wikia.com/wiki/Charmeleon">Charmeleon</a></td>

		</tr>
		<tr>
			<td><img src="http://img1.wikia.nocookie.net/__cb20140328191525/pokemon/images/thumb/3/39/007Squirtle.png/200px-007Squirtle.png"></td>
			<td>Squirtle</td>
			<td>Water</td>
			<td><a href="http://pokemon.wikia.com/wiki/Wartortle">Wartortle</a></td>
		</tr>
		
	</tbody>

</table>
```
## Form
```
<form action="http://www.wikipedia.org">
	<input name="username" type="text" placeholder="username">
	<input name="password" type="password" placeholder="password">
	<input type="submit">
</form>
```
## Radio and Select
```
<form>
	<label for="dogs">Dogs: </label>
	<input name="petChoice" id="dogs" type="radio" value="DOGS">

	<label for="cats">Cats:</label>
	<input name="petChoice" id="cats" type="radio" value="CATS">

	<p>What's your current mood?</p>

	<select name="mood">
		<option value="happy">:)</option>
		<option value="neutral">:|</option>
		<option value="sad">:(</option>
	</select>	

	<input type="text">

	<textarea rows="10" cols="10"></textarea>

	<button>Go!</button>
</form>
```
# CSS
## Color
```
	color: purple;
	color: #F400DD;
	color: rgb(240, 100, 87);
```
```
	color: rgba(0,200,100, 0.8);
	/*border-color: purple;*/
	/*border-width: 5px;*/
	/*border-style: solid;*/
	border: 2px solid rgb(255,100,80);
```
```
h4 {
	background: rgb(255,100,80);
}

body {
	background: pink;
	/*background: url(http://www.graphicsbeam.com/wp-content/uploads/2013/03/Drawn-Wood-Grain-Texture-520x301.jpg);*/
	/*background-repeat: no-repeat;*/
	/*background-size: cover;*/*/
}
```
```
.completed {
	text-decoration: line-through;
}
```
## Selector 
```
li {

}
/*class*/
.hello {

}
/*id*/
#name {

}

/*Star*/

* {
	border: 1px solid lightgrey;
}

/*Descendant Selector*/

li a {
	color: red;
}

/*Adjacent Selector*/

h4 + ul {
	border: 4px solid red;
}


/*Attribute Selector*/

a[href="http://www.google.com"] {
	background: blue;
}

/*nth of type*/

li:nth-of-type(odd){
	background: purple;
}
```
## font
```
/*font-family*/

p {
	font-family: Arial;
}

h1 {
	font-family: Georgia;
}

/*font-size*/

body {
	font-size: 10px;
}
/*font-weight*/

p{
	font-weight: normal;
}

/*line-height*/

p {
	line-height: 1.5;
}

/*text-align*/

h1 {
	text-align: right;
}

p {
	text-align: center;
}

/*text-decoration*/

p {
	text-decoration: underline;
}

h1 {
	text-decoration: line-through;

```
## Box
```
p {

/*Content - Width and Height*/

width: 50%;
/*Border*/

border: 2px solid blue;

/*Padding*/

/*padding: 10px;*/
padding-left: 40px;

/*Margin*/
/*margin: 100px;*/
/*margin-top: 500px;*/
/*margin: 20px 40px 500px 100px;*/
/*margin: 0 auto 0 auto;*/
margin: 0 auto;
margin: 50px 20px;
}
```
## Tic Tac Toe 
define the vertical and horizontal class, and use  ``td:hover`` class to change the border when hovering.
```
<html>
<head>
	<title>TTT Board</title>
	<style type="text/css">

	h1 {
		text-align: center;
	}

	table {
		margin: auto;
	}

	td {
		width: 100px;
		height: 100px;
	}

	td:hover {
		border: 1px solid grey;
	}

	.vertical {
		border-left: 1px solid black;
		border-right: 1px solid black;
	}

	.horizontal {
		border-top: 1px solid black;
		border-bottom: 1px solid black;
	}

	</style>
</head>
<body>

<h1>Tic Tac Toe</h1>

<table>
	<tr>
		<td></td>
		<td class="vertical"></td>
		<td></td>
	</tr>

	<tr>
		<td class="horizontal"></td>
		<td class="vertical horizontal"></td>
		<td class="horizontal"></td>
	</tr>

	<tr>
		<td></td>
		<td class="vertical"></td>
		<td></td>
	</tr>
</table>

</body>
</html>
```
## Image Gallery 
html
```
<!DOCTYPE html>
<html>
<head>
	<title>Photo Blog</title>
	<link href='https://fonts.googleapis.com/css?family=Raleway:400,800' rel='stylesheet' type='text/css'>
	<link rel="stylesheet" type="text/css" href="photos.css">
</head>
<body>

<p>Colt/Steele</p>

<!-- Massimo Margagnoni -->
<img src="http://c1.staticflickr.com/9/8450/8026519634_f33f3724ea_b.jpg">
<img src="http://c2.staticflickr.com/8/7218/7209301894_c99d3a33c2_h.jpg">
<img src="http://c2.staticflickr.com/8/7231/6947093326_df216540ff_b.jpg">

<!-- Giuseppe Milo -->
<img src="http://c1.staticflickr.com/9/8788/17367410309_78abb9e5b6_b.jpg">
<img src="http://c2.staticflickr.com/6/5814/20700286354_762c19bd3b_b.jpg">
<img src="http://c2.staticflickr.com/6/5647/21137202535_404bf25729_b.jpg">

<!-- GörlitzPhotography -->
<img src="http://c2.staticflickr.com/6/5588/14991687545_5c8e1a2e86_b.jpg">
<img src="http://c2.staticflickr.com/4/3888/14878097108_5997041006_b.jpg">
<img src="http://c2.staticflickr.com/8/7579/15482110477_0b0e9e5421_b.jpg">

<!-- All Photos Licensed Under Creative Commons 2.0 -->
<!-- https://creativecommons.org/licenses/by/2.0/legalcode  -->

</body>
</html>
```
css
```
img {
	width: 30%;
	float: left;
	margin: 1.66%;
}

p {
	font-family: Raleway;
	margin-left: 1.66%;
	font-size: 23px;
	font-weight: 800;
	text-transform: uppercase;
	border-bottom: 2px solid #f1f1f1;
	width: 30%;
	padding-bottom: 20px;
}
```
![alt text][id]

[id]: Blog_Solution/blog.html 
