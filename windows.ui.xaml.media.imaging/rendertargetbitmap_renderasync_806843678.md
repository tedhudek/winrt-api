---
-api-type: winrt method
---
 Video content in a [MediaElement](../windows.ui.xaml.controls/mediaelement.md) or [CaptureElement](../windows.ui.xaml.controls/captureelement.md) can't be captured using [RenderTargetBitmap](rendertargetbitmap.md). That includes capturing frames from within video content.
 Custom Microsoft DirectX content (your own swap chain) inside a [SwapChainBackgroundPanel](../windows.ui.xaml.controls/swapchainbackgroundpanel.md) or [SwapChainPanel](../windows.ui.xaml.controls/swapchainpanel.md) can't be captured using [RenderTargetBitmap](rendertargetbitmap.md).
 Content that's in the XAML visual tree but offscreen won't be captured. Content that's in the tree but with its [Visibility](../windows.ui.xaml/uielement_visibility.md) set to **Collapsed** won't be captured.
 Content that's not directly connected to the XAML visual tree and the content of the main window won't be captured. This includes [Popup](../windows.ui.xaml.controls.primitives/popup.md) content, which is considered to be like a sub-window.
 Content that can't be captured will appear as blank in the captured image, but other content in the same visual tree can still be captured and will render (the presence of content that can't be captured won't invalidate the entire capture of that XAML composition).