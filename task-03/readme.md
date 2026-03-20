# Responsive Grid Layout

## Objective: 
  Create a grid layout that displays multiple items

## Requirements:

- Use CSS Grid to arrange items in three columns on desktop
screens.
- Adjust the grid to stack items in a single column on mobile
devices using media queries
- Ensure consistent spacing and alignment between items.

# Grid layout

```
// Desktop view 

#items{
    display: grid;
    grid-template-columns: repeat(2,600px);    // 2 columns with 600px width each
    height: 100%;
}

// Mobile view

#items{
    display: grid;
    grid-template-columns: repeat(1,400px);  // 1 column with 400px width each
    justify-items:center ;
}
```



## Desktop view

<img width="1659" height="978" alt="Image" src="https://github.com/user-attachments/assets/4a2220bd-1b64-4a3a-bb5c-eeb0fe819967" />


## Mobile view

<img width="395" height="883" alt="Image" src="https://github.com/user-attachments/assets/812985a4-702e-497a-bf25-70bed187306d" />