# CSS Accordion Component


## Objective: 
 Build an accordion where content sections expand and collapse on click


## Requirements:

- Use the checkbox hack (a hidden checkbox input with a label) or the `:target` pseudo-class to control the open/closed state of
each section.
- Apply CSS transitions to animate the expansion and collapse of content areas
- Allow multiple sections to be open simultaneously (if desired) or restrict it to one open section at a time..

## Accordion Component


``` html 

    <main>
            <h1 id="heading-fqa"> FQA </h1>

            <div id="accordion">      <!-- To show the FQA section with open/close dropdown-->
                <card>
                    <input type="checkbox" name="option" id="1" checked/>
                    <label for="1">      <!-- map with input  id-->
                        <div class="question">What if bought product not works</div>
                        <div class="answer">You may contact the support team and get refund/other product</div>
                    </label>
                </card>
            </div>
    </main>

```


## CSS to open close the FQA cards 

``` css 

.answer{ 
    
    position: relative; 
    left: 1em;  
    display: none;      /* answer is not display before user click question */
}

.question{   
    cursor: pointer;    /* change the mouse to pointer for better UX */
    border-bottom:1px solid rgb(255, 170, 0) 
}

input:checked+label .answer{
    display:flex;    /* reveal the answer once checkbox is clicked */
}


```


# Desktop view

https://github.com/user-attachments/assets/b9968055-ecd3-4d10-bbe0-5cf959b9b2c9


## Mobile View


<img width="408" height="742" alt="Image" src="https://github.com/user-attachments/assets/3a0972a4-0262-49a9-b9bd-f0dc4f7a9539" />

<img width="405" height="625" alt="Image" src="https://github.com/user-attachments/assets/dad5f86b-50ac-4f15-aedb-a2212d0d716a" />



