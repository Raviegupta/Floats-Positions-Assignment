## Things Learnt

* use of Floats
    * The float property is used for positioning and formatting content
    * `float: left, right, none, inherit`
        * inherit :-  The element inherits the float value of its parent.

* use of clear
    * The CSS clear property specifies what elements can float beside the cleared element and on which side.
    * When we use the float property, and we want the next element below (not on right or left), we will have to use the clear property.
        * `clear : left, right, both, none,inherit`

#### Note :- When clearing floats, we should match the clear to the float: If an element is floated to the left, then we should clear to the left. Your floated element will continue to float, but the cleared element will appear below it on the web page.

    ```
        .div3 {
            float: left;
            padding: 10px;  
            border: 3px solid #73AD21;
        }

        .div4 {
            padding: 10px;
            border: 3px solid red;
            clear: left;
        }
    ```

---
### The clearfix Trick
* If a floated element is taller than the containing element, it will "overflow" outside of its container. We can then add a clearfix hack to solve this problem:

    ```
        .clearfix::before , .clearfix::after{
            content : "";
            display: block, table;
            clear: both;
        }
        
    ```
---
* use of Arrow to navigate to other section of page
    ```
        <section class="arrow">
            <a href="#nav_bar">&#8593;</a> 
        </section>
    ```
        * then use css positioning to fix it.
---
