Page: Modules | Navigation


# Navigation menus

Contao offers you great freedom when it comes to creating navigations on a website. Eight different modules with their own options help you to cover almost every way you could think of to lead visitors to the information they are looking for. A big part of the navigation of a site tree based CMS with nested pages is the concept of start and stop levels.

Let's try to get a little insight into this concept and explain what can be accomplished with Contao.

## Example site structure

* Home
* Music
  * Genres
    * Rock
    * Pop
  * Artists
    * Mrs. X
    * Mrs. Y
* Movies
  * Genres
      * Action
      * Fantasy
  * Actors
    * Mr. X
    * Mr. Y
* Contact


## Default navigation menu

By default, the navigation menu module simply displays the whole site structure. Whenever you add a page to the site tree it will automatically appear in this list.

## Stop level set to 1

If you set the stop level to 1, the navigation menu will only display the first level and all activated pages. Here is what the navigation menu looks like when you are viewing the page Music -> Genres -> Pop.

* Home
* Music
  * Genres
    * Pop
    * Rock
* Movies
* Contact

## Stop level 1 with hard limit

If you want to display even less pages in the navigation menu, you choose the new option "hard limit". That way the navigation menu never shows any page beyond the stop level no matter wether they are activated or not. The ouput is exacly the same as with the "navigation main menu items" module. However, by being able to set a stop level of your choosing, you are not limited to the first level anymore as with the "navigation main menu items" module!

* Home
* Music
* Movies
* Contact

## Stop level 2 with hard limit

A lot of people have requested a navigation menu that allows them to show the first two levels as horizontal main navigation menu and the other levels as optional vertical submenu. You can now accomplish that with the combination of the stop level set to 2 and „hard limit“ enabled.

* Home
* Music
  * Genres
  * Artists
* Movies
  * Genres
  * Actors
* Contact

## Start level 1

The "navigation submenu items" module basically displays the navigation menu from the second level, using the current main menu item as the starting point. Now you can accomplish the same structure with the navigation menu by simply setting the start level to 1. Here is how the navigation menu looks like on the page Music -> Genres -> Pop.

* Genres
  * Pop
  * Rock
* Artists
  * Mrs. X
  * Mrs. Y

## Start level 2

If your main navigation menu includes the first two levels, but you also want your submenu to start with an offset of two levels you have to set the start level to an equivalent 2. Here is how the navigation menu looks like on the Pop page.

* Pop
* Rock
