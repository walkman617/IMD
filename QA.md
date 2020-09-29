## 1. Question: What's the differece between '@+id/' and 'android:id'?
## Answer: 
- The at-symbol (@) at the beginning of the string indicates that the XML parser should parse and expand the rest of the ID string and identify it as an ID resource. 
- The plus-symbol (+) means that this is a new resource name that must be created and added to our resources (in the R.java file). 
- There are a number of other ID resources that are offered by the Android framework. When referencing an Android resource ID, you do not need the plus-symbol, but must add the android package namespace, like so:
<strong>android:id="@android:id/empty"</strong>