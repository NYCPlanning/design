# ![alt text](https://github.com/NYCPlanning/design/blob/edit-readme/assets/readme/nyclogo.png)

A repository for the Design team in the Geographic Data and Engineering team of the NYC Department of City Planning.

## Table of Contents

### In this `design` repo

Files that live in the `design` repo.

- [Streetscape: Foundational Building Blocks Overview](https://github.com/NYCPlanning/design/blob/main/streetscape-foundation-overview.md)

- [Streetscape + Storybook Installation Guide](https://github.com/NYCPlanning/design/blob/main/streetscape-storybook-installation-guide.md)

- [Storybook Designs Plug-In Guide](https://github.com/NYCPlanning/design/blob/main/storybook-designs-plugin-guide.md)

### In Figma

Refer to the Getting Started for an overview on how Figma is used for Streetscape. 

- [Streetscape: Getting Started](https://www.figma.com/design/mfEZjCGYOX49VKyptVDLG6/Getting-Started?node-id=0-1&t=NCfWTwVqMCMt1hen-1)

## Design Glossary

**Design System** - A set of building blocks and standards that help keep the look and feel of products and experiences consistent.

**Design Token** - An industry term to refer to reusable values that are ment to help design and code stay in sync. Typically they define things like typography, color, spacing, and etc.

***Streetscape*** - NYC DCP's design system to align designers and developers for best practices to create consistent and assessible digital products.

**Figma** - Designers' sandbox to create building blocks and standards for *Streetscape*.

**Figma Component** - Elements in Figma that can be reused across your designs.

**Storybook** - Developers' sandbox to workshop UI elements to align with *Streetscape's* standards by using design tokens.

**Storybook Component** - Elements in Storybook that can be reused across implementation.

**Story** -  An interactive state of a Storybook Component. A Storybook Component contains a set of stories (i.e. a button can have three stories: one where the button is inactive, when a user hovers, and when the button is activated).

![alt text](assets/readme/image-1.png)

## Guidelines for Documentation in `design`

### Organizing our repository

Our GitHub repository and project (git issues) serves as a source of truth for documentation. To keep our workflow organized, we will layout some guidelines on how we structure file management and writing guides in `design`.

### Managing files

Edits to existing files should be done in their respective branches before pushing those changes to the `main` branch. For example, if I edit the design readme, I would go to `edit-readme` branch and create my changes here. Once changes are ready, create a pull request and if the changes are good to go, merge to `main`.

> [!IMPORTANT]
> Currently, we are using Pull Requests as our changelog to things related in `design`.
> ![alt text](https://github.com/NYCPlanning/design/blob/edit-readme/assets/readme/prexample.png)

### Writing a markdown

Our current preferred md flavor is GitHub Flavored Markdown (GFM) as most documentation is read in GitHub. [Here is a link to a useful resource on writing in GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github). Additionally, if editing md in VS code, having extensions like [mdlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) can help with syntax.

For content, a brief summary and outline of goals in the beginning is always recommended to provide readers insight on what this documentation entails. The use of visual aids such as images, gifs, and other assets are up to the writer to decide what methods help articulate their points.

### GitHub project and issues

We have one GitHub project where all tasks management lives. Each task is a git issue, which serves as a point of reference for that respective task as they contain notes about research and progression. Issues are tagged by labels that determine what context are related to a task. Issues are also tagged by priority and effort to estimate the scope of a task.

![alt text](https://github.com/NYCPlanning/design/blob/edit-readme/assets/readme/gitissueexample.png)

> [!TIP]
> GFM syntax can be used in Git Issues.

General rule of thumb for issues is to outline summarize shortly what task entails along with goals/to-do in the description. For comments that are outdated or resolved, you should have the ability to collapse them to keep a cleaner progress timeline.
