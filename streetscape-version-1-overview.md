# Streetscape 1

Building the foundation for our design system to sync designers and developers workflows to create consistent and accessible digital products.

> [!IMPORTANT]
> Although the sections below are broken into designers and developers portions for easy reference, it is encouraged for everyone to take the time to understand and learn the different parts that contribute to Streetscape.

## For Designers

### Figma: Libraries and Design Tokens

Within Figma, we have established six foundational libraries that contain design styles respective to their category. Each style contain a design token, which are reusable values used to sync design and development. The importance of design tokens is it establishes collective agreement on design decisions, speeding up the design and development process.

All Figma files related to Streetscape live in the Streetscape project.

![alt-text](https://github.com/NYCPlanning/design/blob/streetscape-v1/assets/streetscape-v1/streescape%20figma%20project.png)

To learn more about how to access and update libraries when working on a design file as well as overall how Figma is used, refer to [Streetscape: Getting Started](https://www.figma.com/design/mfEZjCGYOX49VKyptVDLG6/Streetscape%3A-Getting-Started?node-id=0-1&t=cP49FaXFBwrFe1i0-1).

> [!NOTE]
> Each library file within the Streetscape project contains documentation about design decisions and best practices.

### EDDE Redesign: Test and Iterate

The best method to make sure we on the right track with our decision making while developing our libraries was to apply them to a design. Therefore, we applied our libraries to an EDDE redesign. Refer to [EDDE Redesign](https://www.figma.com/design/d9FEjwAyl6Mb4Sep9tPdNt/EDDE-Redesign?node-id=6-108&t=ZUED3d3k3Qltot4j-1) to look at comparison between the previous and current design.

## For Developers

### Storybook: Upgrading to Version 7.6.2

Updating to the latest 7 version of Storybook to implement Storybook Designs Plug-In, a feature that allows us to embed Figma files into a Storybook component.

### Storybook: Designs Plug-In

We have created a [Storybook Designs Plug-In Guide](https://github.com/NYCPlanning/design/blob/main/storybook-designs-plugin-guide.md) detailing the reasons behind incorporating this feature, demonstrating its capabilities, and outlining how to use the plug-in.

Here is a quick snippet from the guide:

> The Storybook Designs plug-in allows us to embedd figma files into Storybook components. Therefore, when designers create changes to Figma files, it should reflect the new changes within the corresponding Figma file that is embeddeed to its respective Storybook component. This helps bridge the gap between design and implementation as it is easier to see visually what updated Figma components correspond with their Storybook counterpart.

### Design Token Automation


### Figma Dev Mode
