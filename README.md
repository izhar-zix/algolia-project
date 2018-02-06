# Algolia Project

## Description

We have a search database on [Algolia](https://www.algolia.com/doc/). 

Developer documentation on [Algolia can be found here](https://www.algolia.com/doc/).

We'd like to have a drop down search interface on our site search that looks like the image below: 

<img src="https://raw.githubusercontent.com/schappim/algolia-project/master/dropdown-example.png" width=383 style="width:383px!important;"/>

The drop down search interface is to be activated when the user searchs for a product on our website. 

This is an example of a drop down search interface: 
<img src="https://github.com/algolia/autocomplete.js/blob/master/examples/basic.gif"  width=383 />

Please note the search result rows should have the following structure: 

<img src="https://raw.githubusercontent.com/schappim/algolia-project/master/example-row.png" width=383 style="width:383px!important;"/>

A static HTML page `index.html` has been provided for you to code against.

## Requirements

- The dropdown should have the text "Products" as a header
- Your code should be disabled when used on a mobile device, and should not interfer with the exisiting search system. I.e. the search box should fall back to the exisitng search system.
- Hitting the "return key" when content is in the search box should fall back to the existing search system. 
- Clicking anywhere on a result row should take the user to the content in the `handle` key.
- The matched strings should be bold. 
  - A class in the css called ".matched" should be used so it is easy to change the formatting in the future
- Images should be included in the dropdown.
  - The search results provide a link to the full quality version of the image e.g.: `https://www.littlebirdelectronics.com.au/assets/full/PL-2191.jpg`. This needs to be changed client side to `https://www.littlebirdelectronics.com.au/assets/thumb/PL-2191.jpg` where `full` has been replaced with `thumb`.
  - Images should preserve original aspect ratio.
- The content from the `"sku"` key should should be included (where the price is in the attached example).
- A maximum of 12 results should be shown at any time.


## Deliverables

- Code should be checked (in a working state) into this repository
- Javascript and CSS files that achieve the above.


## Important Information 


- Index name: **lbe-products**
- Application ID: **U34J99QLYK**
- Search Only API Key: **54ffd9b3efb53d49a130a7acdbe8742c**

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
