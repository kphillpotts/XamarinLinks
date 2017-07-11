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

#Links {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

#Links li a {
  border: 1px solid #ddd;
  margin-top: -1px; /* Prevent double borders */
  background-color: #f6f6f6;
  padding: 12px;
  text-decoration: none;
  font-size: 18px;
  color: black;
  display: block
}

#Links li a.header {
  background-color: #e2e2e2;
  cursor: default;
}

#Links li a:hover:not(.header) {
  background-color: #eee;
}
</style>
</head>

This is a hand curated list of resources categorised into various topics.

If you have any additional links (or categories) you think should be included please feel free to shoot me an email at kphillpotts@gmail.com and if it's a quality resource I'll add it in.

Search <input type="text" id="myInput" onkeyup="myFunction()" placeholder="Search for links.." title="Type in a link">


<div id="Links">


  * <div class="link">bob <a href="#">something</a><div hidden>ios</div></div>
  * <div class="link">[**The Task-based Asynchronous Pattern**](https://www.microsoft.com/en-us/download/details.aspx?id=19957) - This document provides an in-depth look at the new Task-based Asynchronous Pattern (TAP) for the .NET Framework. By Stephen Toub</div>

* [**Async and Await - Stephen Cleary**](http://blog.stephencleary.com/2012/02/async-and-await.html) - Stephen Cleary provides a high level overview of Async and Await (good introduction)

* [**Asynchrony in C# 5 Part Six: Whither async?**](https://blogs.msdn.microsoft.com/ericlippert/2010/11/11/asynchrony-in-c-5-part-six-whither-async/) - A discussion by Eric Lippert about where the Async keyword comes from.

* [**Parallel Processing and Concurrency in the .NET Framework**](https://msdn.microsoft.com/en-us/library/hh156548(v=vs.110).aspx) - MSDN documentation on threading and asynchronous programming models. 

* [**EduAsync**](https://codeblog.jonskeet.uk/category/eduasync/) - 20 part blog series by Jon Skeet that goes through the ins and outs of Async

* [**Task and TaskCompletionSource**](http://blogs.microsoft.co.il/pavely/2013/04/12/task-and-taskcompletionsource/)
Reporting Progress from Async Tasks

* [**Reporting Progress from Async Tasks**](http://blog.stephencleary.com/2012/02/reporting-progress-from-async-tasks.html) - Stephen Cleary shows how a background process can report progress.

## Videos
* [**Asynchronous Programming with Xamarin**](https://tv.ssw.com/6522/asynchronous-programming-with-xamarin-filip-ekberg-at-xamarin-hack-day-sydney) - In this presentation, Filip Ekberg, C# and Xamarin MVP, gives us a real practical demo of Async and Await in Xamarin.

* [**Six Essential Tips for Async**](https://channel9.msdn.com/Series/Three-Essential-Tips-for-Async) - Channel 9 MSDN video series by Lucian Wischik goes through some essential tips for using Async.  He also has a summary [here](https://blogs.msdn.microsoft.com/lucian/2013/11/22/talk-async-best-practices/).

## Books
* [**Concurrency in C# Cookbook**](http://stephencleary.com/book/) - Stephen Cleary's book on Concurrency. Jon Skeet says: "*The ideal reference book for modern .NET concurrency*" and if it's good enough for Jon, it's good enough for me!

* [**Threading in C#**](http://www.albahari.com/threading/) - Joseph Albahari has a free ebook on his site, which goes into lots of awesome details on threading

</div>

<script>
function myFunction() {
    var input, filter, ul, li, a, i;
    input = document.getElementById("myInput");
    filter = input.value.toUpperCase();
    console.log(filter);
    var ul = document.getElementById("Links");
    var links = document.getElementsByClassName('link');
    
    for (var i = 0; i < links.length; i++)
    {
    	if (links[i].innerText.toUpperCase().indexOf(filter) > -1) 
        {
            links[i].style.display = "";
        } 
        else 
        {
            links[i].style.display = "none";
        }

    }

}
</script>