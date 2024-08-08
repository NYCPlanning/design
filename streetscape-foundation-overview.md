# Streetscape: Foundational Building Blocks

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

### Storybook: Designs Plug-In

We have created a [Storybook Designs Plug-In Guide](https://github.com/NYCPlanning/design/blob/main/storybook-designs-plugin-guide.md) detailing the reasons behind incorporating this feature, demonstrating its capabilities, and outlining how to use the plug-in. All implementation related to Designs plug-in live in [`ae-streetscape`](https://github.com/NYCPlanning/ae-streetscape).

Here is a quick snippet from the guide:

> The Storybook Designs plug-in allows us to embedd figma files into Storybook components. Therefore, when designers create changes to Figma files, it should reflect the new changes within the corresponding Figma file that is embeddeed to its respective Storybook component. This helps bridge the gap between design and implementation as it is easier to see visually what updated Figma components correspond with their Storybook counterpart.

Currently, we have all Storybook components linked to their Figma Chakra UI counterpart on Streetscape's Storybook.

### Design Token Automation

We tried to investigate if it would be possible to automate syncing design tokens from Figma to Storybook. After some progress, we we're blocked by the hurdle to converting our token json file to typescript to comply with Chakra. For more details of this exploration, refer to this [git issue](https://github.com/NYCPlanning/design/issues/34) and this [pr](https://github.com/NYCPlanning/design/pull/39) from `design`.

> ![alt-text](https://github.com/NYCPlanning/design/blob/streetscape-v1/assets/streetscape-v1/design-system-sync.drawio.png)

### Figma Dev Mode

As an alternative to the design token automation, we looked into incorporating [Figma's Dev Mode](https://www.figma.com/dev-mode/) as it contain features that create better handoffs between designers and developers.

Potential features to explore:

- [Annotations in Dev Mode](https://help.figma.com/hc/en-us/articles/20774752502935-Add-measurements-and-annotate-designs-in-Dev-Mode)

> - Highlight important properties so developers can't miss them
> - Help developers quickly visualize specs like spacing and sizing
> - Share additional context with text notes

![alt-text](https://github.com/NYCPlanning/design/blob/streetscape-v1/assets/streetscape-v1/devmodeannotations.png)

- [Code Connect](https://help.figma.com/hc/en-us/articles/23920389749655-Code-Connect)
  - compatible with Storybook and React, [Code Connect Repo](https://github.com/figma/code-connect)

> Use Code Connect to link your components in code with your design system in Figma, so code snippets are always production-ready...bring your design system component code directly into Figma's Dev Mode. Preview example components that mirror the framework of your production code.
>
> "Code Connect is the feature that we’ve been most excited about. Setting it up was super easy– it only took one engineer two weeks."
>

> [!NOTE]
> Code Connect is only available for Organization or Enterprise Figma plans.

## Next Steps

As we established the foundation for our design system, our next steps is to continue to iterate and modify our building blocks to ensure they work in tandem with our current and future products.

### Goals

- Explore how we would like to set up the web components library in Figma. Would it be project specific or a foundational library? How would Chakra UI influence the direction of this library?

- Practice using Dev Mode as default standard for handoff between designers and developers. Therefore, investigating how to incorporate dev mode features would be a good starting point.

  > Here is an example of dev mode in the EDDE redesign:
  > ![alt-text](https://github.com/NYCPlanning/design/blob/streetscape-v1/assets/streetscape-v1/devmodeexample.gif)
  
- Encourage to keep Streetscape updated and have more rigorious testing to comply with WCAG AA and AAA standards.
