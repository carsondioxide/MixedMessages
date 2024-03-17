# Mixed Messages Project

## Contents:

* img folder : contains images of each of the zodiac signs
* `index.html` : because of the lack of server-side communication, the initial content is displayed and the content to be displayed upon user input is set with display style 'none' which is updated via script.js
* `script.js`
  * `createRandomMessage()` : creates and displays the user's random message given the zodiac sign
    * `messageOptions` object : contains arrays of pieces of the random message and getters which return random elements from those message pieces arrays
    * uses `Node.js` to create the new elements to render to the screen
  * `star_signs` array : contains strings representing each of the zodiac signs
  * `controller` : an `AbortController` object to remove the click event listeners from all of the zodiac images once one is chosen
* `style.css` : the style sheet which contains styling for all of the elements and is overridden by the `script.js` file to display the user's horoscope

## Known Issues:

Choosing one sign does not save the information so refreshing the page and choosing the same sign will not necessarily display the same daily message.

## Features to Add:

The ability to either select a zodiac sign OR to enter a birthday which will determine the user's sign.
