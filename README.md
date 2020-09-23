<div align="center">

## Scrolling Menu


</div>

### Description

PLEASE RATE THIS SCRIPT!!! This script will keep the menu on a certain part of your page when the user scrolls. It can be configured for an immediate scroll or a delayed and smoother scroll.
 
### More Info
 
This script is only Internet Explorer 4 and up compatible. I will make it Netscape 6 and up compatible soon, and maybe Netscape 4 and up.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Jim Salyer](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jim-salyer.md)
**Level**          |Beginner
**User Rating**    |4.5 (27 globes from 6 users)
**Compatibility**  |
**Category**       |[Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/menus__2-89.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jim-salyer-scrolling-menu__2-2801/archive/master.zip)

### API Declarations

Look in the code.


### Source Code

```
<html>
<head>
<title>Floating Menu</title>
<script language="Javascript">
<!--
function ScrollMenu()
{
	var menuLeft  = 5;
	var menuTop   = 10;
	var scrollDelay = 100;
	if (document.all.menu.style.pixelLeft < document.body.scrollLeft + menuLeft)
	{
		document.all.menu.style.pixelLeft++;
		setTimeout('ScrollMenu()', scrollDelay);
	}
	else if (document.all.menu.style.pixelTop < document.body.scrollTop + menuTop)
	{
		document.all.menu.style.pixelTop++;
		setTimeout('ScrollMenu()', scrollDelay);
	}
	else if (document.all.menu.style.pixelLeft > document.body.scrollLeft + menuLeft)
	{
		document.all.menu.style.pixelLeft--;
		setTimeout('ScrollMenu()', scrollDelay);
	}
	else if (document.all.menu.style.pixelTop > document.body.scrollTop + menuTop)
	{
		document.all.menu.style.pixelTop--;
		setTimeout('ScrollMenu()', scrollDelay);
	}
}
-->
</script>
<style type="text/css">
<!--
body            { margin-left:5px; margin-top:10px; background-color:white; font-family:Verdana; font-size:12px; font-style:normal; font-weight:bold; text-decoration:none; color:black; }
a:link, a:active, a:visited { text-decoration:underline; color:black; }
a:hover           { text-decoration:underline; color:silver; }
-->
</style>
</head>
<body onScroll="ScrollMenu()">
<div id="menu" style="position:absolute; left:5px; top:10px; width:100px; background-color:maroon; border:2px solid black; padding:2px;">
<a href="link1.htm">Link 1</a><br>
<a href="link2.htm">Link 2</a><br>
<a href="link3.htm">Link 3</a><br>
<a href="link4.htm">Link 4</a><br>
<a href="link5.htm">Link 5</a>
</div>
<div style="height:1000px; width:1000px;"></div>
</body>
</html>
```

