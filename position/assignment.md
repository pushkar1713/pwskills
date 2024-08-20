1. Task 1

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .container {
        position: relative;
        width: 200px;
        height: 200px;
        background-color: #e0ffff;
      }

      .box {
        position: absolute;
        width: 50px;
        height: 50px;
        background-color: #90ee90;
        display: flex;
        justify-content: center;
        align-items: center;
      }

      .a {
        left: 75px;
        top: 75px;
      }

      .b {
        left: 45px;
        top: 45px;
      }

      .c {
        right: 45px;
        top: 45px;
      }

      .d {
        left: 45px;
        bottom: 45px;
      }

      .e {
        right: 45px;
        bottom: 45px;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="box a">A</div>
      <div class="box b">B</div>
      <div class="box c">C</div>
      <div class="box d">D</div>
      <div class="box e">E</div>
    </div>
  </body>
</html>
```

2. Task 2
   Ans.

The difference between Absolute and Relative positioning:

Absolute positioning:

Removes the element from the normal document flow
Positions the element relative to its nearest positioned ancestor or the initial containing block
Other elements act as if the absolutely positioned element doesn't exist

Relative positioning:

Keeps the element in the normal document flow
Positions the element relative to its normal position
Does not affect the position of surrounding elements

3.  Task 3
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .card {
        border: 1px solid #ccc;
        border-radius: 8px;
        font-family: Arial, sans-serif;
        overflow: hidden;
      }

      h2 {
        background-color: #f0f0f0;
        margin: 0;
        padding: 10px;
        font-size: 18px;
      }

      .content {
        padding: 10px;
        overflow: hidden; /* Clearfix */
      }

      .float-right {
        float: right;
        width: 40%;
        margin-left: 10px;
        margin-bottom: 5px;
      }

      p {
        font-size: 14px;
        line-height: 1.4;
        margin: 0;
      }
    </style>
  </head>
  <body>
    <div class="card">
      <h2>The Earth!!!</h2>
      <div class="content">
        <img
          src="https://bgr.com/wp-content/uploads/2022/03/AdobeStock_194080021.jpeg?quality=82&strip=all"
          alt="Earth landscape"
          class="float-right"
        />
        <p>
          Nature is Earth's masterpiece, a symphony of life composed through
          millennia. Its landscapes whisper tales of ancient mountains, winding
          rivers, and flourishing forests, reminding us of the planet's
          boundless beauty. From delicate petals to towering peaks, each element
          plays a vital role in the intricate tapestry of existence. Nature is
          Earth's masterpiece, a symphony of life composed through millennia.
          Its landscapes whisper tales of ancient mountains, winding rivers, and
          flourishing forests.
        </p>
      </div>
    </div>
  </body>
</html>
```

4. Task 4

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sticky Header Example</title>
    <style>
      body {
        margin: 0;
        font-family: Arial, sans-serif;
      }

      header {
        position: sticky;
        top: 0;
        background-color: #333;
        color: white;
        padding: 10px 20px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        z-index: 1000;
      }

      .logo {
        font-weight: bold;
        font-size: 1.2em;
      }

      nav a {
        color: white;
        text-decoration: none;
        margin-left: 20px;
      }

      .cta {
        background-color: #f0ad4e;
        padding: 5px 10px;
        border-radius: 5px;
      }

      main {
        padding: 20px;
      }
    </style>
  </head>
  <body>
    <header>
      <div class="logo">LOGO</div>
      <nav>
        <a href="#">Home</a>
        <a href="#">Pricing</a>
        <a href="#">Contact</a>
        <a href="#">Terms and Condition</a>
        <a href="#" class="cta">Get Started</a>
      </nav>
    </header>
    <main>
      <h2>Heading 2</h2>
      <p>Lorem ipsum dolor sit amet... (repeat for multiple paragraphs)</p>
      <h3>Heading 3</h3>
      <p>Lorem ipsum dolor sit amet... (repeat for multiple paragraphs)</p>
    </main>
  </body>
</html>
```

5. Task 5
   Ans.
   The z-index property in CSS controls the stacking order of elements that overlap. It only works on elements with a position value other than static (e.g., relative, absolute, fixed, or sticky).
   Here's an example to demonstrate z-index:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      .box {
        width: 100px;
        height: 100px;
        position: absolute;
        border: 2px solid black;
      }

      .box1 {
        background-color: red;
        top: 0;
        left: 0;
        z-index: 3;
      }

      .box2 {
        background-color: green;
        top: 30px;
        left: 30px;
        z-index: 2;
      }

      .box3 {
        background-color: blue;
        top: 60px;
        left: 60px;
        z-index: 1;
      }
    </style>
  </head>
  <body>
    <div class="box box1">Box 1</div>
    <div class="box box2">Box 2</div>
    <div class="box box3">Box 3</div>
  </body>
</html>
```
