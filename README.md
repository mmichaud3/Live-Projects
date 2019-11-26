# Live Projects

## Introduction
During my time at The Tech Academy I had the oppurtunity to work with my peers as part of a team of developers to update and create fully functional websites. We all got to spend time on both front and back-end.

## Projects
* [Python Project](#python-project)
* [C Sharp Project](#c-sharp-project)

## Python Project
For my Python project we built and improved on a travel site which had many features.  For my part of this project I spent most of my time on creating a page that would return some brief information about a country and the country's flag.

### Front-End
Here I created a container in which a flag from the searched country would display along with some info on the country.
```
.world_container{    
display: flex;    
width: 100%;    
height: 400px;    
padding: 1%;    
flex-wrap: wrap;    
margin: auto;    
flex-direction: row;
}
.world_form{
    display: inline-block;
    margin: auto;     
    width: 370px;
    height: 300px;
    position: absolute; 
    left: 35%; /*This moves the row box left or right on the page based on the percentage you use */
    background-color: lightgray;
    font-family: 'Montserrat';
    font-size: 20px;
    font-weight: bold;
    /* For a 3D raised effect */
    line-height: 1em;
    /* margin: 1em 2em; */
    border: 6px outset #9a9;
    box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
    -webkit-box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
    -moz-box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
}
.worldInfo{
    display: inline-block;
    margin: 0 auto;
    background: azure;
    width: 370px;
    height: 300px;
    position: absolute;
    left: 69%; /*This moves the row box left or right on the page based on the percentage you use */ 
    padding-top: 20px;
    padding-bottom: 20px;
    font-size: 20px;
    font-weight: bold;
    text-align: center;
    /* For a 3D raised effect */
    line-height: 1em;
    /* margin: 1em 2em; */
    border: 6px outset #9a9;
    box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.4);
    -webkit-box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.4);
    -moz-box-shadow: 5px 5px 15px rgba(0, 0, 0, 0.4);
}

.world_Btn{
   margin-left: 65px;
   margin-top: 50px;
   color: black;
   background-color: #17a2b8;
   font-size: 13px;
   text-decoration: none;
   font-weight: bold;
   cursor: pointer;
   padding: 0px 40px;
   text-shadow: 0px 3px 4px rgba(0, 0, 0, .25);
}



.world_h3 {
    font-family: 'Montserrat';
    color: black;
    text-align: center;
}


 h1 {
    text-align: center;
  }
  #countries-container {
    width: 502px;
    margin: 30px auto;
    padding: 0;
    background-color: lightgray;
  
    text-align: center;
    /* For a 3D raised effect */
    line-height: 1em;
    /* margin: 1em 2em; */
    border: 6px outset #9a9;
    box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
    -webkit-box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
    -moz-box-shadow: 5px 5px 15px rgba(0,0,0,0.4);
   
  }
  #flag-container {
    height: 252px;
    background-color: #fff;
    border: 1px solid #333;
  }
  #flag-container img {
    display: block;
    width: 100%;
    height: 100%;
  }
  #countries-info-container select {
    display: block;
    margin: 20px auto;
    padding: 5px;
    min-width: 100%;
    color: #333;
    font-size: 15px;
    font-weight: 900;
    text-align-last: center;
    border: 1px solid #333;
  }
  #info-container p {
    padding: 0 10px;
    font-weight: 600;
  }
  #info-container p span {
    font-weight: normal;
  }
  
  @media (max-width: 768px) {
    body { font-size: 12px;}
         
    #main-container { width: 342px; }  
    #flag-container { height: 172px; }  
    #info-container select { font-size: 12px; font-weight: 600; }
  }
  ```
### Back-end
This code would allow the user to search a country using Rest API and get back some basic info.
```
{% block content %}
{% include "sidePanel.html" %}
<div class="appContainer">
     <div class='header'>
        <h1>Find Information On The Country You Are Interested In Traveling To!</h1>
     </div>
        <div id="countries-container"> 
            <div id="flag-container">
                <img src="" alt="">
            </div>
            <div id="countries-info-container">
                <select id="countries"></select>
                <p><strong>Capital:</strong> <span id="capital"></span></p>
                <p><strong>Languages:</strong> <span id="languages"></span></p>
                <p><strong>Dialing Code:</strong> <span id="dialing-code"></span></p>
                <p><strong>Population:</strong> <span id="population"></span></p>
                <p><strong>Currencies:</strong> <span id="currencies"></span></p>
                <p><strong>Region:</strong> <span id="region"></span></p>
                <p><strong>Subregion:</strong> <span id="subregion"></span></p>

            </div>
        </div>

    
</div>
```
## C Sharp Project
For this project we created a site for a construction company which allowed for scheduling and assinging employees to jobs.  I worked mostly on front-end tasks.

### Front-End
Here I was tasked with updating a header to make it sticky as well as add some animation to the logo.
```
For making header sticky and adding animation
        #header-title img {
            width: auto;
            height: 75px;
            margin-left: -50px;
            margin-top:-25px;
            position: fixed;
            z-index: 4;
        }
/*******makes header sticky*******/
.float-panel {
    width: 100%;
    background: white;
    opacity: 0.9;
    z-index: 300;
    transform: translateZ(0);
    transition: all 0.5s;
}
    .float-panel .container {
        max-width: 900px;
        margin: 10px auto;
    }
    .float-panel a {
        font-size: 16px;
        text-decoration: none;
        color: #444;
        display: inline-block;
        padding: 10px 20px;
    }
    .float-panel #header-title img {
        
        font-size: 30px;
        /*vertical-align: middle;*/
        transition: all 1s;
    }
 /*Float Panel: class="float-panel fixed"*/ 
.fixed {
    width: 100%;
    box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    padding: 4px 10px;
    animation: slide-down 0.7s;
    opacity: 0.9;
}
/* Animation on logo*/
    .fixed #header-title img {
        transform: rotate(360deg);
    }
@keyframes slide-down {
    0% {
        opacity: 0;
        transform: translateY(-100%);
    }
    100% {
        opacity: 0.9;
        transform: translateY(0);
    }
}
		
    <link href="https://fonts.googleapis.com/css?family=Vollkorn+SC&display=swap" rel="stylesheet" /> <!-- Link for the brand/company title font-->
    @Styles.Render("~/Content/css")
    @using Microsoft.AspNet.Identity;
    @Scripts.Render("~/Scripts/float-panel.js")
    
</head>
<body>
    @if (User.Identity.IsAuthenticated)
    {
        
        <div id="header-nav">   
            <div class="float-panel fixed" data-top="40" data-scroll="200">
                <header class="container">
                    @*<img id="site-header">*@
                    <div class="card-img-overlay" id="left-half">
                    </div>
                </header>
            </div>
        </div>
```
Here I made a shopping cart view more user friendly.
```
.body-content {
    padding-left: 15px;
    padding-right: 15px;
    padding-bottom: 50px;
}
/* Override the default bootstrap behavior where horizontal description lists 
    border: 2px solid white;
    border-radius: 50%;
    width: 35px;
    height: 35px;
    margin-left: 15px;
    margin-right: 20px;
    margin-top: -5px;
}
/*Universal h2 styles*/
        width: auto;
        height: 45px;
        margin-top: -5px;
        margin-left: -15px;
    }
/*Moved the main container over to the right so that it was not being overlapped by the Navbar*/
    padding: 0 10px 0 10px;
    border-radius: 20px;
    background: rgba(255, 255, 255, 0.80);
    width: auto;
}
/* End Mobile - Shopping Cart page */
```
### Back-end
Here I made a table display shift times for employees.
```
@model IEnumerable<ManagementPortal.Models.ShiftTime>
@{
            /**/
            ViewBag.Title = "Index";
            Layout = "~/Views/Shared/_Layout.cshtml";
}
<h2>Shift Times</h2>
<div class="defaultContainer mx-auto" style="text-align: center; width:1000px; ">
    <p>
        <a type="button" class="btn buttonbackground" href="@Url.Action("Create")">
            <i class="fa fa-plus-square"></i> Create New
        </a>
    </p>
    @foreach (var item in Model)
    {
        <div class="card mx-auto " style="width: 810px; margin-bottom: 10px;  text-align: center;">
            <div class="card-body">
                <h5 class="card-title">@Html.DisplayFor(modelItem => item.Job.JobTitle)</h5>
                <div class="card-text">                 
                        <table class="table table-striped table-bg table-hover">                           
                            <tr>
                                <th scope="col">
                                    @Html.DisplayNameFor(model => model.Default)
                                </th>
                                <th scope="col">
                                    @Html.DisplayNameFor(model => model.Monday)
                                </th>
                                <th scope="col">
                                <th scope="col">
                                    @Html.DisplayNameFor(model => model.Sunday)
                                </th>
                                <th scope="col"></th>
                            </tr>
        
                            <tr scope="row">
                                <td>
                                    @Html.DisplayFor(modelItem => item.Default)
                                </td>
                                <td>
                                    @Html.DisplayFor(modelItem => item.Monday)
                                </td>
                                <td>
                                <td>
                                    @Html.DisplayFor(modelItem => item.Sunday)
                                </td>
                                <td class="text-right">
                                    <a type="button" style="margin-bottom: 5px;" class="btn btn-sm btn-primary" href="@Url.Action("Edit", new { id = item.ShiftTimeId })">
                                        <span>
                                            <i class="fa fa-pencil"></i> Edit
                                        </span>
                                    </a>
                                    <a type="button" style="margin-bottom: 5px;" class="btn btn-sm btn-primary" href="@Url.Action("Details", new { id = item.ShiftTimeId })">
                                        <span>
                                            <i class="fa fa-list"></i> Details
                                        </span>
                                    </a>
                                </td>
                            </tr>
                    </table>
                </div>
            </div>
        </div>
    }
   
</div>
```
