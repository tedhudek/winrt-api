---
-api-id: M:Windows.ApplicationModel.Search.SearchPane.Show(System.String)
-api-type: winrt method
---

<!-- Method syntax
public void Show(System.String query)
-->

# Windows.ApplicationModel.Search.SearchPane.Show

## -description
Shows the search pane with the specified initial query string.

## -parameters
### -param query
The initial query string.

## -remarks
> [!NOTE]
> An app can't use both the search box ([Windows.UI.Xaml.Controls.SearchBox](../windows.ui.xaml.controls/searchbox.md) for Windows Store app using C++, C#, or Visual Basic, [WinJS.UI.SearchBox](http://msdn.microsoft.com/library/58f5cea3-a19b-48a8-abcc-17f38d8fa886) for Windows app using JavaScript) and the [SearchPane](searchpane.md). Using both the search box and the search pane in the same app causes the app to throw an exception with this message: "Cannot create instance of type 'Windows.UI.Xaml.Controls.SearchBox.'"

If the search pane is already being shown, this function gives focus to the search pane.

## -examples

## -see-also
[SearchPane class](searchpane.md), [SearchPane.Show() method](searchpane_show_392493604.md), [SearchPane.VisibilityChanged event](searchpane_visibilitychanged.md), [SearchPane.Visible property](searchpane_visible.md)