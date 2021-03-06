---
-api-id: T:Windows.UI.Xaml.Data.CurrentChangingEventArgs
-api-type: winrt class
---

<!-- Class syntax.
public class CurrentChangingEventArgs : Windows.UI.Xaml.Data.ICurrentChangingEventArgs
-->

# Windows.UI.Xaml.Data.CurrentChangingEventArgs

## -description
Provides data for the [CurrentChanging](icollectionview_currentchanging.md) event.

## -remarks
The [CurrentChanging](icollectionview_currentchanging.md) event occurs when the [CurrentItem](icollectionview_currentitem.md) property value changes in an [ICollectionView](icollectionview.md) implementation. The [ICollectionView](icollectionview.md) implementation uses the [CurrentChangingEventArgs](currentchangingeventargs.md) constructor to specify whether you can cancel the [CurrentItem](icollectionview_currentitem.md) change in a [CurrentChanging](icollectionview_currentchanging.md) event handler. If the [IsCancelable](currentchangingeventargs_iscancelable.md) property value is **true**, you can cancel the [CurrentItem](icollectionview_currentitem.md) change by setting the [Cancel](currentchangingeventargs_cancel.md) property to **true**. Otherwise, you cannot cancel the [CurrentItem](icollectionview_currentitem.md) change.

## -examples
The following code example demonstrates how to handle the [CurrentChanging](icollectionview_currentchanging.md) event. In this example, the XAML shows the content of a page with a [GridView](../windows.ui.xaml.controls/gridview.md) bound to a [CollectionViewSource](collectionviewsource.md). The code-behind shows the [CollectionViewSource](collectionviewsource.md) initialization, which includes setting its [Source](collectionviewsource_source.md) and retrieving its [View](collectionviewsource_view.md) in order to attach the [CurrentChanging](icollectionview_currentchanging.md) event handler.



[!code-xml[Xaml](../windows.ui.xaml.data/code/CurrentChangingExample/csharp/BlankPage.xaml#SnippetXaml)]

[!code-cs[Code](../windows.ui.xaml.data/code/CurrentChangingExample/csharp/BlankPage.xaml.cs#SnippetCode)]

## -see-also
[XAML data binding sample](http://go.microsoft.com/fwlink/p/?linkid=226854), [Data binding in depth](http://msdn.microsoft.com/library/41e1b4f1-6caf-4128-a61a-4e400b149011)
