# Metadata: Designing User-Friendly Content

Collaborating with Data Engineering to create easy digestable metadata for DCP data products. Our current MVP is to create new metadata for PLUTO.

> [!NOTE]
> Related Git issues: [assist DE data documentation](https://github.com/NYCPlanning/design/issues/37), [Metadata: Required content for a README](https://github.com/NYCPlanning/design/issues/55)

## Context

The Data Engineering (DE) and GIS teams make and distribute data. In most cases, documentation is made and distributed along with the data and must change to reflect changes in the data.

That documentation is currently manually created and modified. The current forms of documentation which distributed with data are:

- excel files
- PDFs
- text files

The Data Catalog in the DE wiki has links to the destinations these data products and their documentation are distributed to.

## Goals

DE would like to minimize or eliminate the manual modifying of data documentation. In, general, DE would like to:

- create templates of data documentation
- use the new data product metadata to populate templates

This is an opportunity to standardize and improve the design of data documentation.

> [!IMPORTANT]
> Some documentation has strict formatting rules (e.g. data dictionaries in the Attachments of on Open Data pages). But we can determine the form and content of all other documentation.

## MVP: Design Metadata for PLUTO

### Research

The Design team looked into various metadata sources to understand what type content should be prioritized as well as how they should be visually represented (i.e. branding, information hierarchy) within our metadata.

We primarly based off our [inital outline with DE](https://github.com/NYCPlanning/design/issues/55#issuecomment-2271931994) using [USGS Metadata Questionnaire](https://d9-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/atoms/files/MetadataQuestionnaire_508compliant.pdf) and [Metadata in Plain Language](https://d9-wret.s3.us-west-2.amazonaws.com/assets/palladium/production/s3fs-public/atoms/files/Metadata%20in%20Plain%20Language_508compliant.pdf).

Other sources to look into include:

- [FDGC Metadata](https://www.fgdc.gov/metadata)
- [Intro to Metadata](https://www.castordoc.com/blog/what-is-metadata)
- [NASA MODIS Product Data Dict](https://mcst.gsfc.nasa.gov/l1b-documents)

### Figma Wireframes

We created wireframes of how the PLUTO README should be displayed. Wireframes live in `Data Engineering + Design` Figma project space. DE is currently investigating on exporting the CSS styles from Figma to be implemented.

- [Wireframes](https://www.figma.com/design/TrZT5EEaomB8NxOTkAqT7G/Metadata-Redesign?node-id=0-1&t=tp8SZPVFnWeWPzVr-1)
- [Figma API Doc](https://www.figma.com/developers/api)

![alt-text](https://github.com/NYCPlanning/design/blob/metadata/assets/metadata/plutowireframes.png)
