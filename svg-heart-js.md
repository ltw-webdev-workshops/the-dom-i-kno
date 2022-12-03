---
layout: slide-deck
title: "SVG ♥ JS"
desc: "Make a little mouse-interactive SVG graphic with some JavaScript."

slides:
  - type: super-big-text
    content: |
      **SVG ♥ JS**

  - content: |
      ## What & why

      To make really fun & interesting visual interactions SVG can be very helpful.

      SVG is best when combined with HTML, CSS & JavaScript—together the foursome can create magical things.

      **Understanding how to manipulate SVG elements with JavaScript can make great interactions.**

  - type: figure
    video: "https://videos.learntheweb.courses/playlists/web-dev-js/svg-heart-js.mp4"
    caption: "**Moving dinosaur egg**"

  - content: |
      ## Set up

      1. *This is an individual coding activity*
      2. [**Fork & clone this repo**](https://github.com/ltw-webdev-workshops/svg-heart-js/fork)
      3. [**Download the assets**](https://assets.learntheweb.courses/workshops/the-dom-i-kno/svg-heart-js-download.zip)
      4. We’re going to work together, but independently, to each create an interactive SVG

  - content: |
      ## The process:

      We’ll walk through each question together and come up with a solution for each individual carousels.

      1. What HTML & CSS are necessary?
      2. What should the JavaScript do?
      3. Make the JS do its thing!

  - content: |
      ## What HTML & CSS are necessary?

      - How do we export the SVG?
      - How do we insert the SVG into the HTML?
      - How do we control the egg’s position?
      - How do we animate the egg from position to position?

      **Code out the necessary HTML & CSS.**
    numbered: 1

  - content: |
      ## What should the JavaScript do?

      - When does the egg move from side-to-side?
      - What manipulations to the HTML need to be made?
      - What manipulations to the CSS need to be made?

      **Write, in English, what the JS is doing.**
    numbered: 2

  - content: |
      ## Make the JS do its thing!

      - What order does the code need to be in?
      - What elements in the HTML need to be selected?
      - What CSS classes need to be manipulated?

      **Write, in a new JS file, the necessary code.**
    numbered: 3

  - type: two-col-code
    col1:
      jq: |
        // Select an HTML tag; using CSS selectors
        $('.dino')

          // Add a class to an element
          .addClass('move')
          // Remove a class from an element
          .removeClass('move')

          // Calculate the width of an element
          .outerWidth()
    col2:
      jq: |
        // When the mouse is moved on an element
        $('.dino').on('mousemove', function (eventObj) {

          // The current x coordinate of the mouse on the element
          eventObj.clientX

        });

        // Code branching: if-statement
        if (location < 10) {
          // True path
        } else {
          // False path
        }
      jq_lines:
        - num: 10
          text: |
            Logical comparisons:

            - `==` — “is equal to”
            - `!=` — “is not equal to”
            - `<` — “less than”
            - `>` — “greater than”
            - `<=` — “less than or equal to”
            - `>=` — “greater than or equal to”

  - content: |
      ## Helpful links

      - [JavaScript cheat sheet](/topics/javascript-cheat-sheet/)
      - [jQuery API Quick Reference »](https://oscarotero.com/jquery/)

---
