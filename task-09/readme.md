# Complex Responsive Layout with Grid and Flexbox


## Objective: 
  Design a sophisticated webpage layout that combines
CSS Grid and Flexbox techniques

## Requirements:

- Use CSS Grid to structure the main layout and Flexbox to handle
the alignment and spacing of inner elements.
- Create overlapping elements (using `position`  and  `z-index` ) and dynamic reordering based on viewport size.
- Implement a sticky header or sidebar that remains visible as the
user scrolls.


## Complex Responsive Layout with Grid and Flexbox


``` html 
 <!-- Nav bar  -->
     <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li class="has-sub"><a >Brands</a>
                    <ul class="sub">
                        <li><input type="radio" class="sub-opt" name="option" id="1" checked> 
                            <label  for="1">
                             <div>Lenova</div>
                            </label>
                        </li>
                         .
                         .
                         .
                        <li><input type="radio" class="sub-opt" name="option" id="3"> 
                            <label  for="3">
                                <div>Sonny</div>
                            </label>
                        </li>
                    </ul>
                </li>
            </ul>
        </nav>

<!-- top -seller z-index sticky card -->

  <aside>      <!-- carousel for top sales -->
      <img id="top-sales-img"src="images/top-sales.png" alt="Top sales items">
            <div id="carousel">
                <div class="group">
                    <div class="card">
                        <img class="card-img" src="images/lenovo-laptop.png">
                    </div>
                     .
                     .
                     <div class="card">
                        <img class="card-img" src="images/sony-headphone.png">
                    </div>
                </div>

                 <div aria-hidden class="group">
                    <div class="card">
                        <img class="card-img" src="images/lenovo-laptop.png">
                    </div>
                   .
                   .
                   .
                </div>
            </div>
        </aside>

<!-- main page -->

 
        <section id="top-main">
            <div id="intro">
              .
              .
              .
            </div>
            <div id="intro-img">
               .
               .
            </div>


        </section>
        <aside>      <!-- carousel for top sales -->
            .
            .
            .
            .
        </aside>
        <section id="bottom-main">

            <div id="shoping-image-overlap">
                <img src="images/Voice-AI-Phone-Ordering.jpg" alt="Voice-AI-Phone-Ordering">
            </div>
                .
                .
                .
             <section id="shoping-process">
           
                 <div class="process-steps">    <!-- Process steps for online orders -->

                   .
                   .
                   .
                
                </div> 
            </section>

        </section>

    <!-- Last section brand carousel  -->

       <section id="last-section">      <!-- carousel for brand names-->
         <div id="carousel-brands">      
                <div class="group-brands">
                    <div class=" card-brand">
                        <img class=" card-brand-img" src="images/brands/lenovo.png">
                    </div>
                    .
                    .
                    .
                      <div class=" card-brand">
                        <img class=" card-brand-img" src="images/brands/hp.png">
                    </div>
                      <div class=" card-brand">
                        <img class=" card-brand-img" src="images/brands/xiomi.png">
                    </div>
                </div>
               
        </div>

    </section>      


```


## CSS Complex Responsive Layout with Grid and Flexbox

``` css 
body{
    .
    .
    .
    /* Grid layout for navbar , main section , footer */
    display: grid;
    grid-template-columns: 3fr 1fr;
    grid-template-rows: auto 1fr auto auto auto;
    grid-template-areas:
    "navbar navbar" 
    "main aside" 
    "bottom-main bottom-main"
    "last-section last-section"
    "footer footer"; 

    overflow-x: hidden;
}

nav{
    grid-area: navbar;    /* grid area name for body identification */
    position: sticky;   /* allow navbar to stick in top */
    top: 0;
    z-index: 10;   /*  to show top of all other components*/
}


aside{
    grid-area: aside;
    .
    .
    position: relative;   /* adjust form orginal position */
    z-index: 11;   
    position: fixed;  /* fixed position avoid scroll on scrolling */ 
   
    top: 3rem;
    .
    .
}


.card{
    display: flex;   /* flex to alling all cards in linear order */
    justify-content: center;
    align-items: center;
   
    animation: slide 20s infinite linear;    /* for carousel animantion */

}

@keyframes slide {    /* to make a card animation for top sales */
    from{
        translate: 0;
    }to{
        translate: -100%;
    }
    
}

```


# Desktop view

https://github.com/user-attachments/assets/3486aaf8-a2b1-41d3-8b85-e982bf9861c3



