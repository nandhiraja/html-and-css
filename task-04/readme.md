
# Pure CSS Dropdown Menu

## Objective: 
 Design a navigation bar with a dropdown submenu that appears on hover

## Requirements:

- Use nested `<ul>` elements for the menu and submenu.
- Employ CSS pseudo-classes like `:hover`  and transitions to create a smooth reveal effect
- Ensure that the menu looks good on both desktop and mobile (consider using a responsive fallback)
        

## `<ul>` 


``` html
<ul id="navbar">
    <li><a href="api/home">Home</a></li>
    <li><a href="api/about">About</a></li>
    <!-- dropdown -->
    <li class="has-sub">
        <a>Products</a>
        <ul class="dropdown">
            <li>Laptop</li>
            <!-- Nested sub dropdown -->
            <li class="has-sub">       
                Mobile   >
                <ul class="nested dropdown">
                    <li>5G</li>
                    <li>4G</li>
                </ul>
            </li>
        </ul>
    </li>
</ul>
``` 

## Visiblility 


``` css
.dropdown{
    position: absolute;
    color: black;
    background-color: aliceblue;
    margin-top:10px;
    min-width: 8rem;
    visibility: hidden;         //  visibility hidden initialy
    padding: 0px;
    opacity: 0;
    transform: translateY(10px); 
    transition: all .4s ease-in;
    }   

```
## transitions  for smooth reveal effect

``` css
 
.dropdown{
    position: absolute;
    color: black;
    background-color: aliceblue;
    margin-top:10px;
    min-width: 8rem;
    visibility: hidden;
    padding: 0px;

   /* trasnition effect to slow smooth visible */

    opacity: 0;     
    transform: translateY(10px); 
    transition: all .4s ease-in;
    }    

```

## :hover effect to show dropdown

``` css
.has-sub:hover > .dropdown{
        opacity: 1;
        visibility: visible;
        transform: translateY(0); 
    }

```


## Pure CSS Dropdown Menu 


<img width="1899" height="515" alt="Image" src="https://github.com/user-attachments/assets/c7c889fc-2ec9-4dde-b163-0fc584c9c24b" />

<img width="1917" height="515" alt="Image" src="https://github.com/user-attachments/assets/9412df40-918d-4001-914b-46c0a8e88296" />

<img width="1902" height="514" alt="Image" src="https://github.com/user-attachments/assets/a3c680b7-b857-4356-89c3-bfe467dcd61a" />