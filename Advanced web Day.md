<html lang="en"><head>
    <meta charset="UTF-8">
    <title></title>
<style id="system" type="text/css">body{}</style><style id="custom" type="text/css"></style></head>
<body marginheight="0"><h2>CSS Master</h2>
<h2>Modern JS</h2>
<h2>D3 And SVG</h2>
<h2>React</h2>
<h1>CSS Animation</h1>
<ul>
<li><p>Introduction to animations with css</p>
<p>  Many UI design needs it .</p>
</li>
<li><p>Example:</p>
<ol>
<li>add context</li>
<li>provide feedback to users</li>
<li>sleight of hand(showing the process)</li>
<li>Button transisions</li>
<li>flash in effect</li>
</ol>
</li>
<li><p>How to trigger animations</p>
<ul>
<li><p>Pesudo-classes </p>
<ol>
<li><p>hover:</p>
<pre><code class="lang-css"> div:hover{
     background:purple;
 }</code></pre>
<p> <strong>use codepen.io</strong></p>
</li>
<li><p>focus: when the cursor hit it , it is focused.</p>
<pre><code class="lang-css"> input:focus{
     color:red;
 }</code></pre>
</li>
<li><p>active: Triggered when an element is being activated by users.</p>
<pre><code class="lang-css"> button:active{
     color:red
 }</code></pre>
<p>Note: distinguish active and focus. active is refering to 
a movement, but focus refers to a state.The moment of clicking to 
some parts triggers active,after cliking,when releasing it,
it becomes focus.</p>
</li>
</ol>
<p>*practice:</p>
<p>html</p>
<pre><code class="lang-html">  &lt;button class='btn'&gt;click me&lt;/button&gt;</code></pre>
<p>css</p>
<pre><code class="lang-css">  body{
      backgroud-color:#fac046;
      font-family:Lato;
      color:white;
  }
  h1{
      text-align:center;
      font-weight:300;
  }
  .btn{
      outline:none;
      border: none;
      cursor: pointer;
      display: block;
      position:relative;
      background-color: #fcad26;
      font-size:16px;
      font-weight:300px;
      color: white;
      text-transform:uppercase;
      letter-spacing :2px;
      padding :25px 80px;
      margin:0 auto;
      border-radius:20px;
      box-shadow:0 6px #efa424;
  }

  .btn:hover{
      box-shadow:0 4px #efa424;
      top: 2px;
  }

  .btn:active{
      box-shadow:none;
      top:6px;
  }
  }</code></pre>
</li>
<li><p>TRANSFORM</p>
<p>let you manipulate the coordinate space of css visual formating
model like move,warp,rotate and scale elements.</p>
<p>  *Translation</p>
<pre><code class="lang-css">  div{
      transform:translateX(-100px) //move the target  to left in 100 px in horizontal
  }
  div:hover{
      transfor:translate(20px,20px);//move down and right compared to its original state.
  }</code></pre>
<p>  *Scaling(Increse x and y directions by several times)</p>
<pre><code class="lang-css">      div{
          transform:scale(2);//expand (the origin is at top left of the object)
          transform:scale(0.5)//shrinking
          transfor:scaleY(2);
          transform:scale(2,0.5);//expand x by 2 and shrink y by 0.5
          transfor-origin:(0,0) let the origin fixied hen scaling;
          transfor-origin:left top;//now the block will scale in right and bottom directions.
      }</code></pre>
<p>  *Rotations</p>
<pre><code class="lang-css">      div{
          transform:rotate(45deg);//clockwise，the origin is at centor
          transform-origin:left top;//we can change the origin manually
          // if exist two transform, like adding a transform scale();
          //the former transform will be overwritten.
          // 90deg==0.25turn
      }</code></pre>
</li>
<li><p>Note of css vendor prefix</p>
<p>  <strong>feel free to use an auto-prefixer to improve the css code </strong></p>
</li>
</ul>
</li>
</ul>
<pre><code>* TRANSITIONS

let us to control the spped when changing css properties.
    1. transition-duration  //10s  5s
    2. transition-property  // scale rotate  translate
    3. transition-timing-function   //quicker and quicker?
    4. transition-delay   // wait for how long to start the transition

    * transition duration
        ```css
            div{
                transition-duration:1s;
            }

        ```
    * transtion-property

        background, opacity, all,transform 

        ```css
            div{
                transition-property:background,border-radius;
                transition-duration:5s,1s;//corresponding to the above order
            }
        ```
    * transition-delay

        ```css
            div{
                transition-property:background,border-radius;
                transition-delay:2s, 0.5ms // also corresponding to the property order
            }
        ```
    * transition-timing-function

    what is the  acceleration curve for the transition?  easings.net
        ```css
            div{
                transition-timing-function:linear//ease-in(faster) ease-out(slower) ease-in-out
            }
        ```

       ** to generate functions by self, visit https:/matthewlein.com/ceaser **

    * Shorthand Transitions(combines codes to one code)

    ```
    transition: background 1.5s ease-in 1;// property duration timing-function delay

     rotate scale position oapcity should better  be transition</code></pre>
<p>Edit By <a href="http://mahua.jser.me">MaHua</a></p>
</body></html>