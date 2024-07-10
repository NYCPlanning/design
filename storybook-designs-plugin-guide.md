# Streetscape + Storybook Designs Plug-In Guide

This is a guide on how to implement the Storybook Designs plug-in for Streetscape. The current instructions are only compatiable for Storybook version 7.x.x or below. 

Need help to install Streetscape + Storybook? Refer to the [Streetscape Storybook Installation Guide](https://github.com/NYCPlanning/design/blob/main/streetscape-storybook-installation-guide.md). 

## What does the Storybook Designs plug-in do?
The Storybook Designs plug-in allows us to embedd figma files into Storybook components. Therefore, when designers create changes to Figma files, it should reflect the new changes within the corresponding Figma file that is embeddeed to its respective storybook component. This helps bridge the gap between design and implementation as it is easier to see visually what updated Figma components correspond with their Storybook counterpart. 

Designs assigns the embedded Figma file into a Design section within the Add-ons portion of the Storybook page. Here we have a Figma component assigned to a Storybook component.

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/designsection.gif)

Within this Design section, there are a couple useful features:

> Figspec allows you to inspect figma components for their css elements.
<div style="width:20%; margin: auto;">

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/figspec.gif)

</div>

> Not only can you have wireframes or components, you can have live prototypes.
<div style="width:20%; margin: auto;">

![alt-text]()

</div>

