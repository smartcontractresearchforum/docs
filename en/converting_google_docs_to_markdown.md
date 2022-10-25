# Converting Google Docs to Markdown

The [Smart Contract Research Forum](https://www.smartcontractresearch.org/) (SCRF) created "Converting Google Docs to Markdown" to guide contributors on how to structure documentation for GitHub and the forum.

## Overview

Contributors need access to Google Docs and Visual Studio Code (VSCode) to follow the process outlined below to format documentation. After this process, documents are uploaded to HackMD and published to the forum or GitHub.

## Install Extensions and Plugins

* Install the Google Docs add-on "[Docs to Markdown](https://workspace.google.com/u/0/marketplace/app/docs_to_markdown/700168918607?hl=en&pann=docs_addon_widget)"
* Install the free [Grammarly](https://grammarly.com/) browser extension
* [Download VSCode](https://code.visualstudio.com/) and install the following plugins:
  * "[Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)"
  * "[Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)"
  * "[Markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)"
  * "[Replace Curly Quotes](https://marketplace.visualstudio.com/items?itemName=jinhyuk.replace-curly-quotes)"

## Formatting, Review, and Conversion

Follow the steps below to format SCRF's documentation:

* In Google Docs, apply the default settings in the dropdown menu under "Normal text"
  * Use "Title" for the name of the document, "Heading 1, 2, etc." for subsections, and "Normal text" for list items or body text
* Upon completion of the Google Doc draft, fix errors reported by Grammarly
* Review the "[SCRF Writing Style Guide](https://github.com/smartcontractresearchforum/docs/blob/main/en/reference_style_guide.md)" to ensure the document follows SCRF's branding language and provisions
* In Google Docs, run the "Docs to Markdown" add-on in the Extensions drop menu
* Copy and paste all the generated markdown into Visual Studio Code
* In VSCode, open the live preview window to see edits as they will appear on the forum or Github
* Run the "Command Pallete" (Ctrl+Shift+P) and choose "Fix all supported markdown violations in the document" and "Replace curly quotes"
* Review the text for any remaining mistakes
* Copy and paste the text to its destination, such as the forum, GitHub or HackMD

## Learn More About SCRF

The Smart Contract Research Forum (SCRF) is a grant-funded organization dedicated to advancing research while serving the web3 space. [Learn](https://github.com/smartcontractresearchforum/docs) more about SCRF, and discover ways to [get involved](https://github.com/smartcontractresearchforum/docs/blob/main/en/content_connecting_with_scrf.md).
