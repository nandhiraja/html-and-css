# CSS Card Component with Hover Effects

## Objective: 
 Build a card that includes an image, a title, and a
description.

## Requirements:

- Style the card with borders, shadows, and padding
- Add a CSS hover effect (e.g., a background color change or
slight scale transformation) with smooth transitions.


## Hover effect for card : 
```
.card:hover{
    background-color: rgb(40, 40, 40);
    transform: scale(1.02);    /* scale up the card on hovering */
    color: white;    
}
.card:hover .card-image{
    transform: scale(0.9);    /* scale down the image while hover */
}
```

## Smooth tranisition:

```
    transition: transform 0.5s ;     /* give smoother transition while hover */ 

```

---
## Media query for responsive UI

```
@media only screen and  (min-width:300px ) {}

@media only screen and  (min-width:800px ) {}

```

# Preview 

## before hover

<img width="1138" height="966" alt="Image" src="https://github.com/user-attachments/assets/6849cfce-fe11-4041-b7fa-0f45b1b75c01" />

## after hover

<img width="1138" height="975" alt="Image" src="https://github.com/user-attachments/assets/04d01d4e-3b4b-4d59-a4dc-2d4f85b4e2e9" />