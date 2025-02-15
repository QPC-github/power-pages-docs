---
title: Edit code with Visual Studio Code for the Web (preview)
description: Learn how to customize pages by using the Visual Studio Code for the Web editor.
author: neerajnandwana-msft
ms.topic: conceptual
ms.custom: 
ms.date: 10/08/2022
ms.subservice:
ms.author: nenandw 
ms.reviewer: ndoelman
contributors:
    - neerajnandwana-msft
    - nickdoelman
    - ProfessorKendrick
---

# Edit code with Visual Studio Code for the Web (preview)

[!INCLUDE[cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

From the design studio, you can edit site code using **Visual Studio Code for the Web**. This feature allows you to edit a single page's content, custom CSS, and custom JavaScript.

Visual Studio Code for the Web provides a free, zero-install Microsoft Visual Studio Code experience running entirely in your browser, allowing you to browse site code and make lightweight code changes quickly and safely. More information: [Visual Studio Code for the Web experience.](https://code.visualstudio.com/docs/editor/vscode-web)

> [!IMPORTANT]
> - This is a preview feature.
> - [!INCLUDE [preview-tags](../includes/cc-preview-features-definition.md)]

:::image type="content" source="media/visual-studio-code-editor/vs-code-demo.gif" alt-text="Demo of using Visual Studio Code for Web to edit Power Pages site.":::

> [!NOTE]
> - First time **Visual Studio Code for the Web** load may take some time as it will be installing required extensions for this feature. 
> - File Create, Delete and Rename operations are not supported. 
> - This feature utilizes **Power Platform Tools** web extension. Web extensions are restricted by the browser sandbox and therefore have limitations compared to normal extensions.
>   - Power Platform CLI is not supported.
>   - Power Platform Tools web extension features are limited to Power Pages code editing experience.
>   - This feature is not available in Government Community Cloud (GCC), Government Community Cloud (GCC High), and Department of Defense (DoD).  Users in these regions will use the code editor in design workspace to make their changes.  More information: [Using the code editor](#using-the-code-editor)

## Edit code available in design studio

Edit code feature will allow users to edit code in following areas:

- [Edit web page code from Pages workspace](#edit-web-page-code-from-pages-workspace)
- [Header template code from Pages workspace](#header-template-code-from-pages-workspace)
- [Edit custom CSS code from Styling workspace](#edit-custom-css-code-from-styling-workspace)

Let's take a look how to edit code using these areas.

### Edit web page code from Pages workspace

When you open Power Pages design studio, you'll see **Edit code** option in Pages menu<sup>1</sup> and upper-right corner of the screen<sup>2</sup>. 

:::image type="content" source="media/visual-studio-code-editor/edit-code-pages.png" alt-text="Edit code from Pages workspace.":::

### Header template code from Pages workspace

Select site header and then select **Edit code** to open code editor.

:::image type="content" source="media/visual-studio-code-editor/pages-header-edit.png" alt-text="Edit code from Pages header.":::

### Edit custom CSS code from Styling workspace

Go to **Styling workspace** and select available custom CSS **Edit code** menu to open code editor.

:::image type="content" source="media/visual-studio-code-editor/edit-code-custom-css.png" alt-text="Edit code from Custom CSS.":::

## Tutorial: Edit site code using Visual Studio Code for the Web

In this tutorial, you'll walk through editing the site code using Visual Studio Code for Web.

### Step 1: Edit site code using Visual Studio Code

1. Open your site in [Power Pages design studio](../getting-started/use-design-studio.md)

1. On the top right corner, select **Edit code**

    :::image type="content" source="media/visual-studio-code-editor/launch-code-editor.png" alt-text="Opening in Visual Studio Code from the design studio.":::

1. Select **Open Visual Studio Code** from the confirmation dialog.

1. Sign in to Visual Studio Code using your environments credentials.

1. Wait for **Power Platform Tools** web extension to initialize, and web page code to load in left-pane.

### Step 2: Update web page code

1. The explorer on the left-side of the screen will load respective customs CSS and custom JS files along with the web page copy content.

    :::image type="content" source="media/visual-studio-code-editor/vscode-file-explorer.png" alt-text="Explorer menu for an untitled workspace showing web files.":::

1. Make changes to the respective files and press ***Ctrl+S*** to save the changes.

1. Go to design studio and select **Sync** to pull all the updates in your current design studio session.

    :::image type="content" source="media/visual-studio-code-editor/sync-code.png" alt-text="Interface to allow user to select Sync button to synchronize changes made in Visual Studio Code to design studio.":::

1. Select **Preview** to see changes on the Power Pages site.

## Using Visual Studio Code for Web or Visual Studio Code desktop

Users can edit, debug, and preview changes to page edits using Visual Studio Code for the Web without needing to use external tools. Visual Studio Code for desktop provides other advanced features for editing all site metadata and integrating with GitHub, frameworks, and continuous integration/continuous development (CI/CD) processes.

| Feature | Visual Studio for Web | Visual Studio Code desktop |
| - | - | - |
| Direct site editing | Yes | No |
| Site metadata editing | Limited to Custom CSS and Web pages | All power pages configuration entities |
| Site preview | Planned | Planned |
| [Power Platform CLI](/power-platform/developer/cli/introduction) support | No | Yes |
| Advanced CPU and storage bound workflow - ReactJS or other framework build tool support | No | Yes |
| GitHub integration with capabilities such as code check-in, check-out, managing conflicts, and merge. | No | Yes |

## Using the code editor

> [!NOTE]
> - Using Visual Studio Code for the Web to edit websites is not supported in Government Community Cloud (GCC), Government Community Cloud (GCC High), and Department of Defense (DoD).  Users in these regions can use the code editor in design studio to make their changes.
> - Regions that support the Visual Studio Code editor will not see the design studio code editor.

To view the source code of the page on the canvas, select the code editor icon &lt;/&gt; in the command bar.

:::image type="content" source="../getting-started/media/code-editor/code-edit-homepage.png" alt-text="The code editor icon.":::

The source code is displayed in the code editor pane at the bottom of the screen. Any changes you made previously will be updated in the source code. To make changes, update the source code and then select **Save**. The changes will be reflected on the canvas.

The code editor supports three docking options: docked on the bottom, docked on the right side, or full-screen edit mode.

The code editor canvas supports HTML editing. To edit JavaScript or custom CSS, select **Edit CSS & JS**, which will take you to the Portal Management app. From there, select the **Advanced** tab to make any edits you want in the JavaScript and CSS sections.


## See also

- [Use Visual Studio Code and Microsoft Power Platform CLI](power-platform-cli-tutorial.md)
