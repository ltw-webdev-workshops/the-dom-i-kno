---
layout: slide-deck
title: "Dino-rmous carousel"
desc: "Create a dinosaur carousel, on your own, with guidance from peers & the teacher."

slides:
  - type: super-big-text
    content: |
      **Dino-rmous carousel**

  - content: |
      ## What & why

      In order to write effective programs we need to be able to piece together things from many disparte sources.

      There are always many ways to solve a problem, we need to determine what pieces of our knowledge apply.

      **Understanding how to combine the many different sources of knowledge leads to effect programming.**

  - content: |
      ## Set up

      1. *This is an individual coding activity*
      2. [**Fork & clone this repo**](https://github.com/ltw-webdev-workshops/dino-rmous-carousel/fork)
      3. We’re going to work together & separately to each create a unique carousel

  - content: |
      ## The process:

      We’ll walk through each question together and come up with a solution for each individual carousels.

      1. How should the carousel look?
      2. How should the carousel function?
      3. What HTML is necessary?
      5. What basic CSS is necssary?
      6. What should the JavaScript do?
      7. Make the JS do its thing!

  - content: |
      ## How should the carousel look?

      - Will it have next/previous buttons?
      - Will it have the navigation dots?
      - Will it have text for each item?

      **Create a very basic wireframe sketch.**
    numbered: 1

  - content: |
      ## How should the carousel function?

      - Will the items slide in? Slide down?
      - Will the items simply replace the previous?
      - Will one item fade into another?

      **Create a very small storyboard.**
    numbered: 2

  - content: |
      ## What HTML is necessary?

      - What tags will be needed?
      - How are the buttons created semantically?
      - Do the `<img>` tags have surrounding `<div>` or `<figure>` tags?

      **Code out the necessary HTML.**
    numbered: 3

  - content: |
      ## What basic CSS is necssary?

      - Do the items need to be `absolute`?
      - Do the items need to be side-by-side?
      - How are the buttons positioned on the screen?

      **Code out the necessary CSS.**
    numbered: 4

  - content: |
      ## What should the JavaScript do?

      - Does the carousel run automatically?
      - What maniplulations to the HTML need to be made?
      - How do the buttons change the slide, CSS-wise?

      **Write, in English, what the JS is doing.**
    numbered: 5

  - content: |
      ## Make the JS do its thing!

      - What order does the code need to be in?
      - What elements in the HTML need to be selected?
      - What CSS classes need to be manipulated?

      **Write, in a new JS file, the necessary code.**
    numbered: 6

  - type: two-col-code
    col1:
      jq: |
        // Select an HTML tag; using CSS selectors
        $('.dino')

          // Add a class to an element
          .addClass('visible')
          // Remove a class from an element
          .removeClass('visible')
          // Add or remove a class
          .toggleClass('visible')
          // Check if an element has a class
          .hasClass('visible')

          // Get an HTML element’s attribute
          .attr('href');
          // Change the element’s attribute
          .attr('data-state', 'hidden');
    col2:
      jq: |
        // Count how many elements are selected
        $('img').length();

        // Get an element’s parent
        $('.dino').parent();
        $('.dino').parents('figure');

        // Find element children
        $('.dino').find('figcaption');

        // Replace HTML inside element
        $('.dino').html('<img src="" alt="">');

        // When an HTML element is clicked
        $('.dino').on('click', function () {
          // Do maniplulations here…
        });

  - type: two-col-code
    col1:
      js: |
        // Make a new variable
        var count = 0;
        // Add onto a variable
        count++;
        // Change a variable
        count = 1;

        // Code branching: if-statement
        if (count < 10) {
          // True path
        } else {
          // False path
        }
      js_lines:
        - num: 9
          text: |
            Logical comparisons:

            - `==` — “is equal to”
            - `!=` — “is not equal to”
            - `<` — “less than”
            - `>` — “greater than”
            - `<=` — “less than or equal to”
            - `>=` — “greater than or equal to”

    col2:
      jq: |
        // Use a variable
        $('.dino').eq(count).attr('src');

        // Combine plain JavaScript with pre-written jQuery functions
        $('.btn').on('click', function () {
          if (count <= 3) {
            $('.dino').eq(count).addClass('thing');
          } else {
            $('.dino:first-child').addClass('thing');
          }
        });

  - content: |
      ## Helpful links

      - [JavaScript cheat sheet](/topics/javascript-cheat-sheet/)
      - [jQuery API Quick Reference »](https://oscarotero.com/jquery/)

---
