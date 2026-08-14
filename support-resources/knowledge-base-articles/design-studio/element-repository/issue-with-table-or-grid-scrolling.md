# Issue with Table or Grid Scrolling

**Summary**: You may experience issues with horizontal and vertical scrolling within tables or grids in the any application, impacting navigation and usability.

### Error behavior

When this issue occurs, you may observe the following behavior:

* Grid or table scrolling (horizontal and vertical) does not function as expected. &#x20;
* You are unable to move across columns or rows using standard scrolling actions. &#x20;
* Scrollbars may not respond properly or fail to move. <br>

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The scrollbar in the grid is dynamic or not properly recognized by the automation tool. &#x20;
* Standard scrolling actions may not be compatible with the application’s UI behaviour. &#x20;

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. Capture the scrollbar element (horizontal or vertical) using the automation tool. &#x20;
2. Use the **Click on Element** action on the captured scrollbar. &#x20;
3. Provide input values to control the scrolling movement: &#x20;

* For example: 90, 0 will scroll horizontally towards the far right. &#x20;
* Reducing the value will move the scrollbar back towards the left. &#x20;

The same approach can be applied for vertical scrolling by adjusting the values accordingly.

