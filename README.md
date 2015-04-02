# justsaladapp-menu
Replication of the features added to the Just Salad LevelUp mobile app menu.

Update Goal:
------------
To condense the menu (http://bardworx.com/JS/LevelUP/Menu/index.html) and nutrition tabs (http://bardworx.com/JS/LevelUP/Nutrition/index.html)
of the app to one menu of items with sliding nutrition label panel.
Additionally, the previous implementation of the nutrition tab opened the label in the device's browser,
rather than within the running app.

Legacy:
-------
* Editing and browser testing done 7/10/14 - 7/28/14. Update pushed 12/09/14 (1.1.0).
* 2015 commits demonstrate a sample of the changes made before the update. Note that the directory structure of this repo
differs from that on the bardworx test server. This has been done for the sake of readability and to reflect the structure
of the app.
* The commented blocks of code that have been left in certain files show intermediate steps in the design process.
Several animations, event handlers, and styles were removed after successful implementation in concern for aesthetics
or performance.

Features Added:
---------------
1. Animated Ribbon
    - Ribbon descends from top-right corner when items in the selected menu category can
    be tapped for their nutritional information.
    
2. Nutrition Slider
    - Tapping most menu items displays a text-based nutrition facts label as a slider.
    - jquery.js-pageslide.min.js code adapted from jquery.pageslide.min.js by Scott Robbin (srobbin.com)
    - The initial design plan was to swipe left to bring up the slider. Once nutrition panels were
    implemented for Dressings, the swipe left proved too imprecise a screen interaction to be used on
    list items of the aesthetically preferable small size. So, the swipe action was universally abandoned
    for a screen tap.
    
3. Selected Category 
    - The selected menu category is highlighted green and snaps to the top of the page.
