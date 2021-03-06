---
title: "Debug Custom Components | MicrosoftDocs"
description: "How to debug a custom component using Fiddler and Native debugging"
manager: kvivek
ms.date: 04/23/2019
ms.service: "powerapps"
ms.topic: "article"
ms.assetid: 18e88d702-3349-4022-a7d8-a9adf52cd34f
ms.author: "nabuthuk"
author: Nkrb
---
# Debug custom components

Once you are done implementing your custom component logic, get started with testing and debugging your custom component using `npm start` command. This builds your custom component and opens it in the local test harness.

> [!div class="mx-imgBorder"]
> ![test harness 1](media/test-harness-1.png "test harness 1")

As shown in the image above, the browser window opens with 4 sections. The custom component is rendered in the left pane while the right pane has **Context Inputs**, **Data Inputs** and **Outputs** sections.

- **Context Inputs** section provides a way to specify the form factor and test the custom component with each form factor (web, tablet, phone). This is especially helpful when the custom component is dependent on a particular form factor capability. In the coming release, you can have the ability to specify the height and width.
- **Data Inputs** section is an interactive UI that displays all the properties and their types or type-groups defined in the manifest file. It allows you to key in the mock data for each property. 
- **Outputs** section renders the output whenever a component's `getOutputs` method gets called.  

     > [!div class="mx-imgBorder"]
     > ![test harness 2](media/test-harness-2.png "test harness 2")

> [!NOTE]
> If you want to modify the `manifest.xml` file or create additional properties, you need to restart the debug process before they appear in the inputs section.

## Test custom components with Mock data

- For field components, you can input value and type for every property defined in your **ControlManifest.Input.xml** as shown below

   > [!div class="mx-imgBorder"]
   > ![test harness 2.5](media/test-harness-2.5.png "test harness 2.5")

- For datasets, you can load a CSV file with test data. It can be manually created or exported in .csv format directly from your environment. Once a valid CSV file is available, it can be loaded as shown below:

   > [!div class="mx-imgBorder"]
   > ![test harness 3](media/test-harness-3.png "test harness 3")

- After loading a CSV file, bind each property defined in your **ControlManifest.Input.xml** to a column in the CSV. This is done by picking the column for each property as shown below:

    > [!div class="mx-imgBorder"]
    > ![test harness 4](media/test-harness-4.png "test harness 4")

- If you don't have any properties defined in your **ControlManifest.Input.xml**, then all the columns get automatically loaded into the harness.

   > [!div class="mx-imgBorder"]
   > ![test harness 5](media/test-harness-5.png "test harness 5")

## Debug custom components using native browsers

You can use the browser’s debugging capabilities to observe the component behavior. Each browser provides you with a debugging tool to help you debug your code natively in the browser. Typically, you can activate debugging in your browser by pressing the **F12** key to display the native developer tool used for debugging.

For example, on **Microsoft Edge**,

- Press **F12** to open the inspector.
- Click on your component
- On the top bar, go to **Debugger**, and then start searching for the component name described in the Manifest file in the search bar. For example, type your component name like `Hello World component`.

     > [!div class="mx-imgBorder"]
     > ![debug-component](media/debug-control.png "Debug component")

> [!NOTE]
> It is always a good practice to set breakpoints on the component's life cycle methods like `init` and `updateView`.

You can also interact with the component locally in real-time and observe elements in the DOM by setting a breakpoint in the sources tab as follows

> [!div class="mx-imgBorder"]
> ![debug-component](media/debug-control-1.png "Debug component 1")

## Fiddler AutoResponder

Use the Fiddler AutoResponder to debug your custom components quickly. Install [Fiddler](https://www.telerik.com/download/fiddler) and follow the steps to configure [AutoResponder](https://docs.microsoft.com/dynamics365/customer-engagement/developer/streamline-javascript-development-fiddler-autoresponder)

### Related topics

[PowerApps component framework API Reference](reference/index.md)<br/>
[PowerApps component framework Overview](overview.md)
