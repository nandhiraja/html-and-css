# Pure CSS Carousel/Slider


## Objective: 
 Develop an image carousel that cycles through slides automatically and/or manually.
 
## Requirements:

- Use CSS animations (`@keyframes`) to create an auto-sliding effect
- Implement manual slide selection using the `:checked` pseudo-class with hidden radio buttons or the `:target` pseudo-class
- Ensure that the slider is responsive and visually engaging.

## carousel cards 

``` html 

    <main>
            <div id="carousel">
                <div id="carousel-cards">
                    <div class='card'>
                        <img class="card-image" src="./image/desktop.png" alt="card-image">
                        <div class="card-title">Laptop</div>
                      
                    </div>

                        .
                        .
                        .
                        .


                    <div class='card'>
                        <img class="card-image" src="./image/mobile.png" alt="card-image">
                        <div class="card-title">Mobile</div>
                    </div>
                </div>



                
                <!-- Dummy card for smoothness -->
                 <div aria-hidden  id="carousel-cards">   
                    <div class='card'>
                        <img class="card-image" src="./image/desktop.png" alt="card-image">
                        <div class="card-title">Laptop</div>
                    </div>

                     .
                     .
                     .
                     .

                    <div class='card'>
                        <img class="card-image" src="./image/mobile.png" alt="card-image">
                        <div class="card-title">Mobile</div>
                    </div>
                </div>
            </div>

        </main>
```


## animation 

``` css 
/*  card alignment */
#carousel-cards{
    ...
    animation: slide 40s infinite linear;        /* use the "slide"  keyframe animation in infinite time  runing  */

}

@keyframes slide {     /* Keyframes  to make animation */

    from{
        translate: 0;
    }
    to {
        translate: -100%;
        
    }
    
}


```


# Desktop view
https://github.com/user-attachments/assets/f417b337-f89a-41f1-8417-e3b6e8e01228



## Mobile View

https://github.com/user-attachments/assets/20392bcf-8eb4-462f-bd7c-f66362f0084f  



