---
title: "Add, move or delete tabs on a form using the form designer | MicrosoftDocs"
ms.custom: ""
ms.date: 04/21/2019
ms.reviewer: ""
ms.service: powerapps
ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "get-started-article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
  - "PowerApps"
author: "Aneesmsft"
ms.author: "matp"
manager: "kvivek"
tags: 
  - "PowerApps maker portal impact"
search.audienceType: 
  - maker
search.app: 
  - "PowerApps"
  - D365CE
---

# Add, move, or delete tabs on a form  
[!INCLUDE [cc-beta-prerelease-disclaimer](../../includes/cc-beta-prerelease-disclaimer.md)]

Add, move, or delete tabs on a form using the form designer.

## Add tabs to a form
To add tabs to a form, use the **Layouts** pane.  

> [!div class="mx-imgBorder"] 
> ![](media/layouts-pane.png "Layouts pane")
   
  > [!NOTE]
  >  Tabs can only be added on main forms. More information: [Form types](types-forms.md)

### Add tabs to a form using drag and drop

1. Open the form designer to create or edit a form. More information: [Create a form](create-and-edit-forms.md#create-a-form) or [Edit a form](create-and-edit-forms.md#edit-a-form)
2. In the command bar, select **Add control**, or in the left pane, select **Layouts**. 
3. In the **Layouts** pane, select a tab control and drag it onto the form preview. As you drag the tab on the form preview, you will see drop targets where you can add the tab. 
4. Drop the tab in the location you want. Note the following: 
    - Tabs can be dropped before or after any existing tabs by hovering over the tab headers.
    - Tabs can also be dropped before or after the current tab by hovering over the left or right edge of the current tab.
5. Repeat steps 3-4 above if you want to add more tabs.
6. In the command bar, select **Save** to save the form, or select **Publish** if you want to save and make your changes visible to users. 

### Add tabs to a form using selection 

1. Open the form designer to create or edit a form. More information: [Create a form](create-and-edit-forms.md#create-a-form) or [Edit a form](create-and-edit-forms.md#edit-a-form)
2. In the form preview, select another existing tab or the form. Note the following:
    - When you select an existing tab, the new tab will be added after the existing tab. 
    - When you select the form, the new tab will be added as the last tab on the form. 
3. In the command bar, select **Add control**, or in the left pane, select **Layouts**.  
4. In the **Layouts** pane, select a tab control to add it to the form. Alternatively, select **...** next to the tab control you want, and then select **Add to form**. 
5. Repeat steps 2-4 above if you want to add more tabs.
6. In the command bar, select **Save** to save the form, or select **Publish** if you want to save and make your changes visible to users. 

## Move tabs on a form

### Move tabs on a form using drag and drop

1. Open the form designer to create or edit a form. More information: [Create a form](create-and-edit-forms.md#create-a-form) or [Edit a form](create-and-edit-forms.md#edit-a-form)
2. In the form preview, select the tab header of the tab that you want to move and initiate the drag action. As you drag the tab on the form preview, you will see drop targets where you can move the tab.  
3. Drop the tab in the location you want. Note the following:
    - Tabs can be dropped before or after any existing tabs by hovering over the tab headers.
    - Tabs can also be dropped before or after the current tab by hovering over the left or right edge of the current tab.
4. Repeat steps 2-3 above if you want to move more tabs.
5. In the command bar, select **Save** to save the form, or select **Publish** if you want to save and make your changes visible to users. 

### Move tabs on a form using cut and paste

1. Open the form designer to create or edit a form. More information: [Create a form](create-and-edit-forms.md#create-a-form) or [Edit a form](create-and-edit-forms.md#edit-a-form)
2. In the form preview, select the tab that you want to move.
3. In the command bar, select **Cut**.
4. In the form preview, select another existing tab or the form.
5. In the command bar, select **Paste** or select the chevron, and then select **Paste before**. Note the following: 
    - When you select **Paste**, the tab being moved is pasted after the existing tab. 
    - When you select **Paste before**, the tab being moved is pasted before the existing tab.
    - When you select the form, the tab being moved is added as the last tab on the form. The **Paste before** action is not applicable and therefore not available in this case.
6. Repeat steps 2-5 above if you want to move more tabs.
7. In the command bar, select **Save** to save the form, or select **Publish** if you want to save and make your changes visible to users. 

## Delete tabs on a form
1. Open the form designer to create or edit a form. More information: [Create a form](create-and-edit-forms.md#create-a-form) or [Edit a form](create-and-edit-forms.md#edit-a-form)
2. In the form preview, select the tab that you want to delete from the form. 
3. In the command bar, select **Delete**.
4. Repeat steps 2-3 above if you want to delete more tabs.
4. In the command bar, select **Save** to save the form, or select **Publish** if you want to save and make your changes visible to users. 

    > [!NOTE]
    >   - Tabs can only be deleted on main forms. More information: [Form types](types-forms.md)
    >   - If you delete a tab by mistake, in the command bar, select **Undo** to revert the form to its previous state. 
    >   - You can't delete a tab that contains sections with required or locked fields. 
    >   - You can't delete a tab that has locked sections. 
    >   - A form must have at least one tab. You can't delete the last remaining tab on the form. 

### See also
[Overview of the model-driven form designer](form-designer-overview.md)  
[Create or edit forms using the form designer](create-and-edit-forms.md)  
[Add, move or delete fields on a form using the form designer](add-move-or-delete-fields-on-form.md)  
[Add, move or delete sections on a form using the form designer](add-move-or-delete-sections-on-form.md)  
[Properties available in the form designer](form-designer-properties.md)  
[Configuring header properties in the form designer](form-designer-header-properties.md)  
[Using the tree view in the form designer](using-tree-view-on-form.md)  
[Create and edit fields](../common-data-service/create-edit-field-portal.md)
