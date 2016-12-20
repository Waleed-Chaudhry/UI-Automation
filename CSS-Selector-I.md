##CSS Selector 

<center><img src="https://github.com/timothyylim/interview-prep/blob/master/perfect-tree.png" width="350"></center>

* Syntax: $(selector)  
* Right click an element on a webpage, and click inspect  
* After inspection, go to console and type: $("input.gsfi") to select the element just inspected

**Basic Selector** 
```groovy

<center><img src="https://github.com/Waleed-Chaudh1ry/UI-Automation/blob/master/css-selector-1.png" width="350"></center>

$("input.gsfi") // input is the tag, gsfi is the name of the class  
$("input#lst-ib") // lst-ib is the id of the element with tag input
$("input[name = 'q'][title = 'Search']") //search using two attributes at once
```

**Partial Text Matching**
```groovy
$("input[class ^= 'gs']") //Class attribute value starts with 'gs'
$("input[class $= 'fi']") //Ends with 'fi'
$("input[class *= 'sf']") //Has 'sf' in the middle
```

**Other syntax**
```groovy
$("input.gsfi.search.textbox") // use in place of class = gsfi search textbox
$("div#gs_lc0")[1] //Select the second child of the element selected by ("div#gs_lc0") 
$("input").size //verify the number of elements matched
clear //clear the consolte
```
