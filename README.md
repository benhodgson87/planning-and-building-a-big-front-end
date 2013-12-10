# Planning and Building a Big Front-End

Today’s workshop is going to be pretty hectic; there’s a lot to get through and
I’m keen not to spend too much time talking at you. Below is a list of things
I’d like to cover and the rough order in which I want to go about it but… Let’s
just enjoy ourselves, freestyle it and hammer out some code! Interrupt me shout
out, open up discussion and let’s have fun!

## Schedule

* Intro
* Setup
    * Get the repo
    * Get Sass working
        * Intro to Sass for any who need it
    * Have a peek round the repo
* Look at the design
    * Rationalise/discuss it
    * Deconstruct it
* Code theory
    * A shift in thought
        * The web has changed
        * The three stakeholders – who we need to keep happy
    * SRP
    * Selectors
    * Specificity
    * Semantics are silly
    * Naming things
    * Naming conventions
    * Shearing layers
* Let’s code!
    * Familiarise ourselves with the codebase
        * This looks huuuuuuge!
        * Look at its structure, what lives where (and why)
    * Using the above, let’s build some stuffs!
    * No layout.
* Layout
    * Layout should be a component unto itself
    * Put all our components into a page
    * Done.
* Questions, recap.

## Source order

1. `settings/` – Variables, feature switches and other project specific
   settings. These are defined first and will be picked up and used by the
  framework later on.
2. `tools/` – Mixins and functions to make tasks easier. These appear early
   on so that they can be utilised in the main body of the codebase.
3. `generic/` – Resets, global `box-sizing`. These styles are really far
   reaching; they underpin every element we place on the page.
4. `base/` – Base elements, unclassed `h1`, `ol`, etc. These are semantic
   HTML elements that require some base styling for when they exist outside of
   a component context (e.g. a regular, bulleted list in some body copy).
5. `objects/` – design patterns, objects, abstractions and constructs.
6. `gui/` – Designed components and modules. These build on top of semantic
   HTML elements and are referred to mainly through class selectors.
7. `trumps/` – Style trumps, helper classes and overrides. These need to
   override any other styles and thus come last. It is not uncommon for these
   styles to carry `!important`.

## Important numbers and values

* Page background color: `#f9f9f9`
* Page text color: `#424242`
* Pink: `#f43059`
* Nav border color: `#e0e0e0`
* Nav grad start: `#fafafa`
* Nav grad stop: `#e1e1e1`
* Grey box grad start: `#535657`
* Grey box grad stop: `#414445`
* Pink button grad start: `#f54469`
* Pink button grad stop: `#d12a4c`
* Pink button border color: `#bd2343`
* Grey button grad start: `#30312f`
* Grey button grad stop: `#292a28`
* Grey button border color: `#1a1b19`
* Solid grey box color: `#e8e1df`
* `h1`:
* `h2`:
* `h3`:
* `h4`:
* `h5`:
* `h6`:
