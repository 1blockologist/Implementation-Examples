# Implementation Examples
Descriptions and visual examples of implementations I've created

## Custom Pull to Refresh

This is a user experience (UX) tweak that diverges away from the common bland pull to refresh visual element that users find in many apps. This implementation allows for more branding and theming to be done where it may not otherwise fit on the layout. A perk here is that more information can also be added, such as words or graphics that tell the user that the application is syncing or loading, while presenting the user with exciting elements to keep their attention and their engagement high.
<p align="center">
  <img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-custom-ptr-tp.gif" height="550">
  </br>##### *Trend Prophet - Stock Market Trading*
</p>

The above example features a tableview (RecyclerView object) with a header. The classical art (seen in the Pull to Refresh drop down) is a key part of the app's theme, but would not fit very well with the aesthetics of the main application state. As part of the tableview header, it would also be too large or not fit well. Adding it into the pull to refresh user experience, and overriding the pull to refresh objects with custom graphics, creates this branding opportunity and adds an extra dimension to the user experience.

## Custom Sticky Headers

Table view headers provide an opportunity to show additional relevant information to the user without putting to much redundant information into each tableview cell.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-custom-sticky-headers-tp.gif" height="550">
	</br>##### *Trend Prophet - Stock Market Trading*
</p>

Here, the tableview cells are tied to a date and also show numbers, but an explanation about which date or what the numbers mean is not a part of the cell's user interface (UI), instead they are all aligned with a column named in the tableview header. This UI allows for less clutter in each cell and gives the user more relevant information that can be seen in a quick glance.

## Stateful Navigation / UI Elements

There are many instances where a lot of functionality is desired that will clutter a screen with static buttons to get the user's attention. UX designers often don't consider element states in their static image designs. Stateful navigation is an improvement to UX where certain visual elements are hidden when they are not relevent to the user. An optimization that the shows or hides information based on what the user is looking at, without requiring the user to touch buttons/symbols that drill them down into other parts of the app.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-statefulnavigation-tp.gif" height="550">
	</br>##### *Trend Prophet - Stock Market Trading*
</p>

## I/O operations without degrading performance