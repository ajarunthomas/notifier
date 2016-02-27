# notifier
jQuery Plugin to push notifications on your webpages
<br>
Developed by Arun Thomas
<br>
www.ajarunthomas.com
<br>
<br>
<a href="http://www.ajarunthomas.com/jquery/notifier/demo/" target="_blank" style="text-decoration:none">Demo</a>
<a download href="http://www.ajarunthomas.com/files/notifier.js" target="_blank" style="text-decoration:none">Download</a>
<br><br>
<a href="http://www.ajarunthomas.com/jquery/notifier/" target="_blank" style="text-decoration:none">Website</a>
##USAGE
###Step 1 : Include JS Files
```
<script type="text/javascript" src="js/jquery-1.12.0.min.js"></script>
<script type="text/javascript" src="js/notifier.js"></script>
```
###Step 2 : Initialize jQuery
```
$(window).load(function(){	
	$.notifier({	
	  "message":"Enter your notification message here",  	//content to be shown in the notification bar
	  "color1":"white",  	//background color of the notification bar	
	  "color2":"black",  	//color of the text	
	  "closeButton":"text",  	//shows a textual close button rather than a cross sign button.	
	  "delay":3  	//when to show the notification from trigger point (in seconds)	
	});	
});
```
###INSTRUCTIONS

The above example will show the notification 3 seconds after the webpage has loaded. If you want to trigger the notification on button click, then include the initialization code inside the jquery click method. 

####EXAMPLE : 
```
$(document).ready(function() {	
  $('#myDiv').click(function(){	
    $.notifier({	
    	"message":"this is your notification"
  	});	
  });	
});
```

If you want to include an image in the notification, the insert the img tag in the message area.

####EXAMPLE : 
```
$.notifier({	
  	"message":"<img src='images/picture.jpg' />"
});	
```
