**CMSI 370** Interaction Design, Fall 2016

# Assignment 1216
We conclude your exposure to direct manipulation implementation with a different type of product—instead of a full application, this time you are asked to build a _reusable component_ that uses direct manipulation.

## Background Reading
The readings from [Assignment 1122](https://github.com/lmu-cmsi370-fall2016/assignments/blob/master/direct-manipulation.md) apply here also.

## For Submission

### Direct Manipulation Widget
We wrap up our programming work by going back to the basics: design and implement a reusable direct maniuplation widget for use in web browsers in general, and for your custom front end in particular. To emphasize reusability, implement your widget as a [jQuery plugin](https://learn.jquery.com/plugins/). Further, you are to provide a _notification mechanism_ (likely in the form of a callback) that informs users of your widget of relevant events, e.g., such as when the widget’s model value changes.

The point here is to see how low-level event handling (e.g., mouse/keyboard/touch activity) translate into higher-level ones (e.g., selection or change events). If [Assignment 1122](https://github.com/lmu-cmsi370-fall2016/assignments/blob/master/direct-manipulation.md) involved direct manipulation “in the large,” this one exercises direct manipulation “in the small.” Some ideas:

- A selection knob or slider
- A rolling or scrolling item selector
- An entry field that accepts text/numbers with drag-and-drop character tiles
- A “here-to-there” drag-and-drop area
- A directional pad (“d-pad”) control

If you have a widget idea that is not in this list, check with me to see if it will work.

You may use jQuery but Bootstrap use must be limited to _CSS only_—no Bootstrap JavaScript components allowed, whether in code or triggered by `data` attributes. To be more precise, aside from jQuery, _all other external JavaScript_ must be cleared by me first. The supplied repository includes three examples of reusable components _in general_, all with callback mechanisms, but only the swivel control fulfills the direct-manipulation, no-Bootstrap-JavaScript specifications of this assignment.

### How to Turn it In
Commit your code in two places. Within _this_ repository, provide:

1. The reusable code for the widget (typically CSS and JavaScript)
1. The unit test suite for the widget (see the supplied sample code for examples)
1. A standalone demonstration page that shows an instance of your widget in action (see the supplied demonstration gallery page for examples)

Under the repository for the web front end assignment:

1. Commit the reusable code again (simulating the scenario where you might have downloaded someone’s widget code for use with your front end), and
1. Integrate your widget into the user interface that you have already built.

Because this assignment involves integration with your web front end, you may rejoin forces with your web front end partner. As before, make sure to show that your work was equitably distributed by way of your commits.
