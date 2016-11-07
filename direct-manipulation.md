**CMSI 370** Interaction Design, Fall 2016

# Assignment 1122

For this assignment, we turn our attention to the _direct manipulation_ interaction style. As before, resources to help you with this include many of the links listed on the course website, assorted samples from the [bazaar](https://github.com/dondi/bazaar) repository, and the starter files that are included with your GitHub Classroom repositories for this assignment, once you have set yourself up.

## Background Reading
Textbook reading is centered on the direct manipulation interaction style, which would be Shneiderman/Plaisant Chapter 5. Additional helpful material outside of the web and the [bazaar](https://github.com/dondi/bazaar) code will be the case studies in Chapter 9 of the JavaScript textbook. These case studies demonstrate lower-level event handling with some direct manipulation elements. Code from that chapter is available on the [JavaScript book’s GitHub repository](https://github.com/dondi/javascript-book/tree/master/chapter09).

## For Submission
This assignment requires access to a multitouch-capable and accelerometer-aware web browser. Most of you already own such a device; if not, arrange to check one out from the Keck lab.

This assignment can be worked on in pairs, preferably someone you have not worked with yet and _definitely_ not the same person from the web front end assignment. Make sure that the work is distributed equitably. Collaborate in a way that ensures a balanced distribution of commits between the two of you.

### A Direct Manipulation Proof-of-Concept
The code in the GitHub Classroom repository is a copy of the [boxes-with-physics](https://github.com/dondi/bazaar/tree/master/boxes-with-physics) sample from the bazaar. Modify this code into one of the following options:

#### A “Live” Box-Drawing App
Convert the supplied code into a “drawing” app where, in addition to the existing functionality, the user can also:
- Create new boxes by dragging their finger(s) across the drawing area.
- Resize boxes that are already present using either the classic “pinch” gesture or an alternative touch interaction of your own design.
- Delete boxes by dragging them to a designated “trash” area.

Optional features (time permitting) include:
- Rotating boxes by turning two fingers around an imaginary _z_-axis.
- Implementing animation changes other than acceleration.
- Implementing drawing choices such as colors and borders.

Box creation and deletion, like box motion, must be fully multitouch-capable: that is, the user should be able to perform the operation concurrently on multiple boxes, limited only by the number of fingers that the device can follow.

#### A Simple Physics-Based Game
Convert the supplied code into something resembling a game that makes use of acceleration and multitouch. Possibilities include:
- A multiplayer air hockey-like game
- A breakout-style game using multiple paddles
- A pinball-style game where the flippers are controlled directly by the player
- An obstacle course game that follows the physical tilt of the device
- A projectile-and-target game where the user can “fire” multiple concurrent projectiles

Other ideas are welcome as long as they use multitouch and device acceleration. The game itself doesn’t have to be mind-blowingly awesome or original—just implemented well.

### Best Practices, Implementation Notes, and Automated Feedback
Remember that this is a _proof-of-concept_ app—focus on the multitouch and acceleration functionality and don’t get lost in refinement and details. Do that _after_ the assignment is due.

The sample code that comes with your GitHub Classroom repository is fully configured for code style review ([ESLint](http://eslint.org)). It will be hard enough to implement this from first principles, and it will be harder still to write unit tests for these, so no test suite is required for this assignment. Test your app manually.

Please note that this aspect of your code _is_ graded. Points will be deducted if issues found by the automated feedback system linger in the final submission, so _don’t ignore it_.

### How to Turn it In
Commit your direct manipulation web app files such that your repository becomes the root location of a web server. To evaluate your work, we will run a simple HTTP server from a local copy of that directory and use your application from a multitouch- and accelerometer-capable web browser.
