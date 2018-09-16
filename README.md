# Project

This is web-based application that reads RSS feeds. The original developer of this application clearly included [Jasmine](http://jasmine.github.io/) and wrote the first test suite ( RSS Feeds - are defined).

## Take a look on the project
To fully understand how Jasmine works, follow the procedures:

1. Download or clone the project
2. Unzip it
3. Open up `index.html`
4. Jasmine tests should be at the end of this file
   Green point means everything is ok.
   Red point means there is something wrong

### Test:
Edit the `allFeeds` variable in **./js/app.js** to make the provided test fail and see how Jasmine visualizes this failure in your application, work to implement the changes and then return the `allFeeds` variable to a passing state.

No test should be dependent on the results of another.

Test for: menu, entries and new feed

# Explanation

Inside the "RSS feeds":
All related to var allFeeds, the data with all the information
* it('are defined'...)| was done by the developer - ensure the feeds are not empty
* it('url defined'...)| - ensure the url are not empty
* it('name defined'...)| - ensure the name are not empty

Inside the "The menu":
Related to the menu performance
* it('menu hiden'...)| - ensure the hiding(by default)/showing performing by Css
* it('menu visible'...)| - ensures the menu changes visibility according to $('.menu-icon-link') one click-show, two clicks hide

Inside the "Initial Entries":
Related to entry element on the Loadfeed
* first the asynchronous, with the beforeEach  to work before the it - calling the Loadfeed
* it('at least one (.entry element...)|- ensure there is at least a single `.entry` element within the `.feed` container.


Inside the "New Feed Selection":
Related to upload of news feed
* first the asynchronous, creating the news feed
* it('new feed loaded'...)| - ensure that the new feed content actually changed
