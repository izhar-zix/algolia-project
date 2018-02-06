# Algolia Project

## Description

We have a search database on Algolia. 
We'd like to have a drop down interface on our site search that looks like the image below: 

<img src="https://raw.githubusercontent.com/schappim/algolia-project/master/dropdown-example.png" width=383 style="width:383px!important;"/>

## Requirements

- The dropdown should have the text "Products" as a header
- Clicking anywhere on a result row should take the user to the content in the `handle` key.
- The matched strings should be bold. 
  - A class in the css called ".matched" should be used so it is easy to change the formatting in the future
- Images should be included in the dropdown.
  - The search results provide a link to the full quality version of the image e.g.: `https://www.littlebirdelectronics.com.au/assets/full/PL-2191.jpg`. This needs to be changed client side to `https://www.littlebirdelectronics.com.au/assets/thumb/PL-2191.jpg` where `full` has been replaced with `thumb`.
  - Images should preserve original aspect ratio.
- The content from the `"sku"` key should should be included (where the price is in the attached example).
  

## Deliverables

- Code should be checked into this repository
- A maximum of 12 results should be shown at any time.
- Javascript and CSS files that achieve the above.


## Important Information 


- Application ID: **U34J99QLYK**
- Search Only API Key: ***54ffd9b3efb53d49a130a7acdbe8742c***

Example Record: 

```
{
      "sku": "PL-2191",
      "title": "Arduino Uno R3",
      "description": null,
      "local_inv": 0,
      "supplier_inv": 0,
      "location": "F.E.3.4",
      "image": "https://www.littlebirdelectronics.com.au/assets/full/PL-2191.jpg",
      "handle": "https://www.littlebirdelectronics.com.au/arduino-uno-r3"
}
```



