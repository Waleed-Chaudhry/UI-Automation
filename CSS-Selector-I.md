##CSS Selector 

* Syntax: $(selector)  
* Right click an element on a webpage, and click inspect  
* After inspection, go to console and type: $("input.gsfi") to select the element just inspected
* $$("input") will bring about all the input tags matching that selector
* Use $$ when you're figuring stuff out  

**Basic Selector** 
```groovy
$("input.gsfi") // gsfi is the name of the class  
$("input#lst-ib") // lst-ib is the 
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
