# Streetscape + Storybook Designs Plug-In Guide

This is a guide on how to implement the Storybook Designs plug-in for Streetscape. The current instructions are only compatiable for Storybook version 7.x.x or below.

Need help to install Streetscape + Storybook? Refer to the [Streetscape Storybook Installation Guide](https://github.com/NYCPlanning/design/blob/main/streetscape-storybook-installation-guide.md).

## What does the Storybook Designs plug-in do?

The Storybook Designs plug-in allows us to embedd figma files into Storybook components. Therefore, when designers create changes to Figma files, it should reflect the new changes within the corresponding Figma file that is embeddeed to its respective Storybook component. This helps bridge the gap between design and implementation as it is easier to see visually what updated Figma components correspond with their Storybook counterpart.

Designs assigns the embedded Figma file into a Design section within the Add-ons portion of the Storybook page. Here we have a Figma component assigned to a Storybook component.

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/designsection.gif)

### Within this Design section, there are a couple useful features

> Figspec allows you to inspect figma components for their css elements.
<div style="width:20%; margin: auto;">

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/figspec.gif)

</div>

> Not only can you have Figma components, you can have live prototypes.
<div style="width:20%; margin: auto;">

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/figmaprototype.gif)

</div>

## How to Install Designs Plug-In

These steps are based of documentation for [Designs v7.0.9](https://github.com/storybookjs/addon-designs/tree/v7.0.9) as it is compatiable with our Storybook version (Storybook 7.6.20).

### 1. Install correct packages

    npm install -D @storybook/addon-designs

    yarn add -D @storybook/addon-designs

    pnpm add -D @storybook/addon-designs

### 2. Check to see if plug-in is registered in `main.tsx`

There should already be `"@storybook/addon-designs"` tag in `addon` parameter of your `main.tsx` file. if not, add the tag in the same format as the other addons.

## Adding an Embedded Figma File to a Storybook Component

### 1. Choosing a Storybook component

Within `ae-streetscape`, traverse down to the `components` folder from `src`. This is where we store all Storybook components and their respective files. Each Storybook component consists of two files, we will specifically focusing on `nameofcomponent.stories.tsx`, which stores the different stories a Storybook Component can have.

> *What is a story?* A story is an interactive state of Storybook component. For example, a button could consist of two stories: one for its inactive state and another its active state when the button is pressed.

### 2. Adding the `design` parameter to a story

To add the figma component to a story, choose the respective story within your `nameofcomponent.stories.tsx` and add the following:

    export const NameofStory: Story = {
        parameters: {
            design: {
                type: "figma",
                url: "paste-figma-url-here",
            },
        },
    };

Notice that for the `type`, we default to `figma`. If you would like to use the figspec feature, that type needs to be changed to `figspec`. More steps for figspec will be explained further down.

### 3. Choosing a Figma component

The type of link you put in the url field will impact what is seen in the embedded Figma file. Here are some choice we have:

> To link a specific Figma component, select to component in Figma. Please make sure to copy using copy link to selection.

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/selectingfigmacomponent.png)

> To link a live prototype, the link must be from the prototype in presentation mode. Go to your respective prototype page on figma and click the play button to launch presentation mode. Next, go to share and copy the figma url.

![alt-text](https://github.com/NYCPlanning/design/blob/designs-plugin/assets/selectingprototype.png)

### Optional: Using Figspec

As we stated above, if you would like to use the figspec feature, that type needs to be changed to `figspec`.

    export const NameofStory: Story = {
        parameters: {
            design: {
                type: "figspec",
                url: "paste-figma-url-here",
            },
        },
    };

Additionally, we need to include your personal figma access token for figspec to work properly. [Follow these instructions from Figma to generate and obtain your token](https://www.figma.com/developers/api#access-tokens).

In `ae-streetscape`, there is a file called `sample.env', this is where we will place our personal access token from figma.

    # use your personal figma access token and local .env file

    STORYBOOK_FIGMA_ACCESS_TOKEN=paste-figma-access-token-here

When you run Storybook locally, be sure to change your `sample.env` file to `.env`.
