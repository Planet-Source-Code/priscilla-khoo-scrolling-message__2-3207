<div align="center">

## Scrolling Message


</div>

### Description

Scrolls message at bottom left of screen. Please vote for me thanks.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Priscilla Khoo](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/priscilla-khoo.md)
**Level**          |Beginner
**User Rating**    |4.5 (18 globes from 4 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/priscilla-khoo-scrolling-message__2-3207/archive/master.zip)





### Source Code

```
<html>
<head>
<title>Scrolling Message</title>
</head>
//Done by Priscilla Khoo
<body>
<script LANGUAGE="JavaScript">
 <!--
 // Scrolling message settings
 var MessageText = "Welcome to Yupigirl's Homepage enjoy!:)"
 var DisplayLength = 130
 var pos = 1 - DisplayLength;
 function ScrollInStatusBar(){
 var scroll = "";
 pos++;
 if (pos == MessageText.length) pos = 1 - DisplayLength;
 if (pos<0) {
 	for (var i=1; i<=Math.abs(pos); i++)
 	scroll = scroll + "";
 	 scroll = scroll + MessageText.substring(0, DisplayLength - i + 1);
 }
 else
  scroll = scroll + MessageText.substring(pos, pos + DisplayLength);
 window.status = scroll;
 //Scrolling speed
 setTimeout("ScrollInStatusBar()",0);
 }
 ScrollInStatusBar()
 //-->
 </script>
</body>
</html>
```

