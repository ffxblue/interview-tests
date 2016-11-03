---
layout: test
title:  Weather Widget
---
The purpose of this exercise is for us to get a sense of how you would approach designing and implementing a simple Javascript widget, before we get you in for an interview. We've tried to focus on something that shows how you would structure a front end solution.

There is no time limit, but we expect most applicants to spend roughly 2-3 hours working on the test. Once complete please share your repository, forward a zip file of the source code and dependencies, or use a service like Dropbox to share the file.

Feel free to use any language/toolset you like. The only requirement is that you can describe how to set it up on a mac so we can see it running.

If you make any assumptions about requirements, or use any online resources to solve a problem, please make note of these somewhere obvious inside the solution (e.g. code comments).

Your solution will be evaluated internally by one or more of your potential co workers. You should expect a response from us within 2 business days.

## Requirements

Create a "weather widget" editor that allows users to set up a widget that can then be embedded on any site.

### Editor

The widget editor must have a form to allow a user to create a new widget. This form must include the following fields:

1.	Title
1.	Unit: metric or imperial
1.	Show Wind: true or false

The widget editor must also display a list of already created widgets with their title and a snippet of code that allows that widget to be embedded.

### Widget

The widget itself should be a piece of Javascript that reads the end user's current location using `navigator.geolocation`, and retrieves the current weather conditions for that location using the [Open Weather Map API](http://openweathermap.org/current).

The data the widget displays is determined by the settings in the editor; i.e. if I created a widget called "Imperial with Wind Data" and chose imperial units, and Show Wind, I should be able to embed that widget and see those two options reflected in the widget display.

### Example

Make an example page within the same solution that shows how the widget can be embedded, and has some CSS to style up the widget appearance. You may choose to use something like https://erikflowers.github.io/weather-icons/.

### Tests

Make sure you have tests covering both the editor, and the widget.

## Deliverables

Please submit the following deliverables to: `blueco DOT tech DOT test AT gmail DOT com`. You will receive a confirmation email for your submission.

1. Source code for the solution described above
1. Setup/installation instructions
1. A quick (1-2 page) description of your solution, outlining anything of interest about the code you have produced. This could be anything from why you chose the language and or libraries, why you structured the project the way that you did, why you chose a particular error handling strategy, how you approached testing etc
1. A list of assumptions that you've made while putting this together. We've only given you a very loose spec, so you'll probably need to fill in some blanks while you are working. If you note down the assumptions, for us, then we will be able review the code within the context of those assumptions
1. [Optional] Tell us what you thought of the test and how long it took you to complete
