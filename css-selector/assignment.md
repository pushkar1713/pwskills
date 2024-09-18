Q1. For the given index.html file. Perform the following task, without changing the index.html file.

Ans :

```css
nav a ｛
color: green;
nav > h2 {
color: red;
background-color: snow;
}
ul +p{
color: red;
}
a[href] {
color: red;
text-decoration: none;
LS
}
a[class="active"] {
color: blue;
text-decoration: underline;
}
a[target="_self"]{
background-color: grey;
}

p:last-child: :after {
content: "...";
}
li: marker {
color: green;
}
p:nth-child(even)::first-letter {
color: red; font-size: 30px;
}
```

Q2. For the given index.html file. Perform the following task, without changing the index.html file.

```css
ul li a {
  list-style: none;
  text-decoration: none;
}
ul > li {
  display: inline;
}
li + li {
  margin: 10px;
}
```

Q3. Using any of the Pseudo element selectors, add any random words after and before the given HTML tag
index.html

Ans :

```css
h1: :after {
  content: "selector";
}
h1 ::before {
  content: "Pseudo";
}
```

Q4. Illustrate ine example of pseudo-class element selector hover example should include the following

Ans :

```css
button {
  background-color: royalblue;
  border: none;
  margin-top: 100px;
  margin-left: 100px;
  padding: 15px 30px;
  color: #ffffff;
  font-size: 18px;
  border-radius: 10px;
}
button:hover {
  box-shadow: 10px 5px 5px grey;
  cursor: pointer;
}
```
