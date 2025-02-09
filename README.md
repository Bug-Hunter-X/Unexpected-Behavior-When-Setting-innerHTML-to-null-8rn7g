# Uncommon HTML Bug: Unexpected innerHTML Behavior

This repository demonstrates an uncommon bug related to using `innerHTML` in HTML.  Setting `innerHTML` to `null` does not remove the element; instead, it only removes its content. This can lead to unexpected layout issues or behavior if not handled correctly. The solution shows the correct approach for removing an element.

## Bug Description
Setting the `innerHTML` property of an element to `null` will clear the content of the element but it won't remove the element itself. This might not be the intended behavior and can lead to subtle issues.  This is not a common mistake, making it somewhat uncommon.

## Solution
The solution uses the `removeChild` method to properly remove the element from the DOM. This is the standard and expected way to delete an element from the page.