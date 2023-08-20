---
title: "Readme"
tags: readme, knowledge, base, internal
date:
  created: "03/21/2022"
  modified: "08/06/2022"
description: Readme page for SAVI Knowledge Base. Contains guidelines for what should be included in each section.
---

<a href="Assets/Knowledge-Base/Creator/Drivers/Logos/savi3-color-dark.png">
  <img src="Assets/Knowledge-Base/Creator/Drivers/Logos/savi3-color-dark.png" alt="SAVI 3 logo" width="600" height="">
</a>

# Readme
* All files should be lower case with dashes (-) in place of spaces. 
* Every markdown page should have a YAML header with the categories included above.
  * The 'modified' field should always be the last date edited, not the date uploaded/merged into the Main git.
* Images should be restricted to a width of '600' or a height of '300'
* KB pages should be structured under `Knowledge-Base`
  * Each category/item should have a `Getting Started` page with an overview.
  * Additional details should be detailed in individual markdown pages.

##### Markdown Commands:
* A basic guide can be found [here](https://www.markdownguide.org/basic-syntax/)
* Comment out: `<!-- -->`
* Line break: `<br>`
* HTML style image link: `<a href="Assets/Knowledge-Base/image-location.png">
  <img src="Assets/Knowledge-Base/image-location.png" alt="Alt text" width="" height="">
  </a>`
* Wrap Around Image: `<img align="right" width="100" height="100" src="https://imagelocation.png">` followed by text after a double line break.


---

### Assets:
* Should mirror the main file structure with media in appropriate locations.
* Prefer PNG images over other file types.
* Non-media files should be placed in the Files directory.

### Documentation:
* All docs should be placed in the Documentation directory (preferably as PDFs).

### FAQ:
* Use collapsible categories for each question and answer.
* Unsure if we want to use HTML page for FAQ.

### Release Notes:
* Only track version 3.1.2 and later.
* Possibly condense hotfix versions and beta versions together into tabs with a page per version number.

### Known Limitations:
* Should have a page for each release separated by product.
* Should summarize categories of limitations rather than detailing each specific one.

---

### Driver Pages:

Example entries:
* **Name:** Name of the device.

* **Location:** Location of the device within the Project. New Locations can be created by selecting this field, typing in a new name, and then selecting the corresponding "Add New Tag" option or pressing Enter on your keyboard.
<img src="Assets/Knowledge-Base/Creator/Drivers/locations-add.png" alt="Adding Main Dining Tag to Location" width="200" height="">

* **IP Address:** The destination IP address that SAVI will use when communicating with the device.

#### Driver Questions for Review: (each driver page answer cover all of these)
* What does this driver control?
* What is the purpose of this driver?
* Can this driver be used by anyone?
* Does this have any required dependencies (other driver, etc)?
* What features does this control?
* What devices does this work with (whole line, single device, etc)?
* Are any inputs/outputs mandatory?
* Are all inputs/outputs usable?


><p style="text-align:center"><b>Warning: This is a test for centering warnings and notes.</b></p>

If using this driver as an Alternate Volume Control, leave all connections blank.
