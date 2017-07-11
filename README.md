# Welcome to XamarinLinks
<head>
<style>
* {
  box-sizing: border-box;
}

#myInput {
  background-image: url('/css/searchicon.png');
  background-position: 10px 12px;
  background-repeat: no-repeat;
  width: 100%;
  font-size: 16px;
  padding: 12px 20px 12px 40px;
  border: 1px solid #ddd;
  margin-bottom: 12px;
}

#myUL {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

#myUL li a {
  border: 1px solid #ddd;
  margin-top: -1px; /* Prevent double borders */
  background-color: #f6f6f6;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  color: black;
  display: block
}

#myUL li a.header {
  background-color: #e2e2e2;
  cursor: default;
}

#myUL li a:hover:not(.header) {
  background-color: #eee;
}
</style>
</head>

This is a hand curated list of resources categorised into various topics.

If you have any additional links (or categories) you think should be included please feel free to shoot me an email at kphillpotts@gmail.com and if it's a quality resource I'll add it in.

Search <input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for names.." title="Type in a name">


<!-- MarkdownTOC depth=4 -->

# Table of Contents
* [Design](#design)
    * [Inspiration](#design-inspiration)

<a name="design"></a>
## Design

<a name="design-inspiration"/>

### Inspiration Sites
* [**Dribbble**](https://dribbble.com/) - Dribbble is show and tell for designers.


## Xamarin.Forms Performance

## Android Layout

# General Development
* [*Async, Await and Threading*](async_await.md)

<script>
function myFunction() {
    var input, filter, ul, li, a, i;
    input = document.getElementById("myInput");
    filter = input.value.toUpperCase();
    ul = document.getElementById("myUL");
    li = ul.getElementsByTagName("li");
    for (i = 0; i < li.length; i++) {
        a = li[i].getElementsByTagName("a")[0];
        if (a.innerHTML.toUpperCase().indexOf(filter) > -1) {
            li[i].style.display = "";
        } else {
            li[i].style.display = "none";

        }
    }
}
</script>