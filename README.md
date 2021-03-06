<a name="intro"></a>
# Implementation Examples
Presented are descriptions and visual examples of implementations I've created. Application development can be an art that offers a myriad of creative opportunity that can improve functionality and the user experience, reducing friction and boosting performance.

<a name="toc"></a>
## Table of Contents

- [Implementation Examples](#intro)
- [Table of Contents](#toc)
- [Custom Pull to Refresh](#custom-pull-to-refresh)
- [Custom Sticky Headers](#custom-sticky-headers)
- [Stateful Navigation / UI Elements](#stateful-nav)
- [I/O operations without degrading performance](#io-operations)
- [Custom Loading Indicators](#custom-loading-indicators)
- [Custom Platform Specific Features](#custom-platform-specific-features)
- [Low Friction Login](#low-friction-login)

## Custom Pull to Refresh

This is a user experience (UX) tweak that diverges away from the common bland pull to refresh visual element that users find in many apps. This implementation allows for more branding and theming to be done where it may not otherwise fit on the layout. A perk here is that more information can also be added, such as words or graphics that tell the user that the application is syncing or loading, while presenting the user with exciting elements to keep their attention and their engagement high.
<p align="center">
  <img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-custom-ptr-tp.gif" height="550">
  </br><i>Trend Prophet - Stock Market Trading - version 0.13</i>
</p>

The above example features a tableview (RecyclerView object) with a header. The classical art (seen in the Pull to Refresh drop down) is a key part of the app's theme, but would not fit very well with the aesthetics of the main application state. As part of the tableview header, it would also be too large or not fit well. Adding it into the pull to refresh user experience, and overriding the pull to refresh objects with custom graphics, creates this branding opportunity and adds an extra dimension to the user experience.

## Custom Sticky Headers

Table view headers provide an opportunity to show additional relevant information to the user without putting to much redundant information into each tableview cell.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-custom-sticky-headers-tp.gif" height="550">
	</br><i>Trend Prophet - Stock Market Trading - version 0.13</i>
</p>

Here, the tableview cells are tied to a date and also show numbers, but an explanation about which date or what the numbers mean is not a part of the cell's user interface (UI), instead they are all aligned with a column named in the tableview header. This UI allows for less clutter in each cell and gives the user more relevant information that can be seen in a quick glance.

<a name="stateful-nav"></a>
## Stateful Navigation / UI Elements

There are many instances where a lot of functionality is desired that will clutter a screen with static buttons to get the user's attention. UX designers often don't consider element states in their static image designs. Stateful navigation is an improvement to UX where certain visual elements are hidden when they are not relevent to the user. An optimization that the shows or hides information based on what the user is looking at, without requiring the user to touch buttons/symbols that drill them down into other parts of the app.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-statefulnavigation-tp.gif" height="550">
	</br><i>Trend Prophet - Stock Market Trading - version 0.13</i>
</p>

<a name="io-operations"></a>
## I/O operations without degrading performance

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/io-android-performance-wst.gif">
	</br><i>WhoSay Talent - version 3.7</i>
</p>

Creating a user experience that doesn't lag is a challenge that requires foresight and pristine application architecture. As we push the design paradigms further, we have more and more data serialization happening as well as image processing and resource recycling. Getting this right requires experience far beyond what provided SDKs will achieve.

This example shows many database queries being executed, as well as garbage collection. These are all I/O operations which can block the UI thread without careful thought, yet there is no blocking occuring to the user due to successful design, despite an ever increasing number of network calls and views being loaded.

## Custom Loading Indicators

It is prudent to consider that even loading indicators can be engagement opportunities for delivering information, entertainment, branding or theming.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-customloading-android-wst.gif" height="550'">
	</br><i>WhoSay Talent - version 3.7</i>
</p>

## Custom Platform Specific Features

Different platforms offer a variety of unique ways to engage with the user. Android offers widgets, which are applications which can display views on the home screen (a.k.a the launcher). Without a deep understanding of "views", it may not be obvious that non-standard shapes can be used to create widgets, as seen in this example:

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-android-widget-ml.gif" height="350">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-widget-android-wsf.gif" height="350">
	</br><i>New York City MapLights Widget (left), WhoSay Fan (right)</i>
</p>

The left widget depicts the different administrative districts (boroughs) of New York City. Each borough in this widget lights up when there is new information posted on the internet about or from those boroughs. They can also respond to touch events independently. Engagement opportunities exist far outside of the common app-in-a-box model when it comes to development on mobile platforms, and it is important to architect applications with an understanding of this.

The widget on the right depicts a custom view within a flip-card widget object provided by the android SDK. Each card also deep links into the full activity process based application.

## Low Friction Login

Give a helping hand. Seemingly small things such as autocompleting a username will help with user engagement.

<p align="center">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-lowfrictionloginA-android-wst.gif" height="550'">
	<img align="center" src="https://github.com/ericlw/Implementation-Examples/blob/master/images/ux-lowfrictionloginB-android-wst.gif" height="550'">
	</br><i>WhoSay Talent - version 3.7</i>
</p>

[back to top](#intro)
