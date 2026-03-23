# Modal Popup Using the `:target`  or Checkbox Hack

## Objective: 
 Build a modal (popup window) that opens and closes without JavaScript.

## Requirements:

- Use an anchor link with an ID and the `:target`  pseudo-class—or a hidden checkbox with the `:checked` pseudo-class—to control
the modalʼs visibility
- Style the modal to appear centered with an overlay backdrop.
- Add CSS transitions for the modalʼs appearance and disappearance.

# Model popup  using :trigger 


## using :trigger
```html
    
    <a href="#cart"> <img id="cart-img" src="image/cart.png"></a>   <!-- #cart will trigger the popup-->

    <!-- inside cart container-->
    <a id="close-btn" href="#">x</a>     <!-- # will trigger to close the  popup-->


```

```css 
#cart{
    .
    .
    .
    display: none;   /* display none to hide the popup initaly */
}

#cart:target{ 
    display: block;        /*  allow to visible cart as popup */
}


```
## Desktop view 

``` css


#cart{
    width: 100%;
    height: 200%;
    background-color: rgba(48, 48, 49, 0.784);
    justify-self:center;
    top: 0px;
    position: absolute;     /* to make oververlap on others  bring forward */
    z-index: 1;      /* make sure card hover effect  not affect the cart view */
    display: none;


}
#model{
    width: 600px;
    height:600px;
    align-self:center;
    justify-self: center;
    background-color: rgb(247, 249, 248);
    border-radius: 30px;
    position: sticky;      /* enable stick on same view */
    top: 20%;               /* top space to aling in center  */
    box-shadow: 10px 100px 400px  black;

}

```

## Mobile view

```css

/*  responsive UI for Movile view cart */
#model{
    width: 300px;
    height: 400px;
}

#close-btn{   /* button to close the cart */
     right:10px;
     font-size: 25px;     /* reduce the font size */
     padding: 3px 10px;    

    }

#title{
    font-size: 30px;
}

```



## Desktop view

<img width="1912" height="982" alt="Image" src="https://github.com/user-attachments/assets/2fbff473-6189-449a-8288-d0361ce71902" />


## Mobile view

<img width="405" height="880" alt="Image" src="https://github.com/user-attachments/assets/0c73ad1b-9400-4010-9e86-5672f028558b" />