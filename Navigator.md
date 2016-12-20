# Navigator

### General Syntax
```groovy
$(<css selector>, index/range, attribute/text matcher) //parameters 2 and 3 are optional
```
**Index/Range**
```groovy
$("p", 2).text() //picks second element with tag p
```

**Attribute/Text Matchers**
```
<p attr1="a" attr2="b">p1</p>
<p attr1="a" attr2="c">p2</p>
```

```groovy
//Attribute Matchers
assert $("p", attr1: "a").size() == 2
assert $("p", attr2: "c").size() == 1
assert $("p", attr1: "a", attr2: "b").size() == 1 //can add multiple attributes at once

//Text Matchers
assert $("p", text: "p1").size() == 1
assert $("p", text: "p1", attr1: "a").size() == 1 //can mix text and attribute matchers
assert $("p", text: startsWith("p")).size() == 2 //ther pattern matchers are on the geb manual
```

**Find**
```
<div class="a">
    <p class="b">geb</p>
</div>
```

```groovy
$("div").find(".b")
//Once you're inside the find paranthesis, you can think of it as having another css selector to begin with
```

* There are other examples such as filter, has, not, hasNot on the manual
* There are also jQuerry style traversing options on the manual 
