# Popup

## Symbol
![image](smd-popup.png)

## Symbol Properties

| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Ref Sitemap Id | String | Refers to the sitemap that represents the popup. This property must correspond with a [Sitemap Id](../smd-sitemap/README.md) within the same project. |
| Ref Page Id | String | Name of the [Page Id](../smd-page/README.md) to be shown. The Page ID must correspond with a [Page Id](../smd-page/README.md) of the [Ref Sitemap Id](../smd-sitemap/README.md). |
| Mandatory | Shadow | Indicates whether or not the referred sitemap will hold the focus until it is closed (indicated by a dark shadow) or that the user can still navigate within the sitemap that triggered the popup, even when the popup hasn’t been closed yet (indicated by a white shadow). |

## Documentation Properties
| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| - | - | - |

## Explanation
The popup symbol represents that another application window. The popup may only be invoked by an [associative link](../smd-associative-link/README.md) and has to be drawn outside of the invoking [sitemap symbol](../smd-sitemap/README.md). 
A sitemap may hold several popups with the same Ref Sitemap Id. Several popups with the same Ref Sitemap Id also refer to the same physical application window.
Opening a popup with the same Ref Sitemap Id than an already opened popup should not open another popup, but should replace the content of the already open popup window with the content of the newly opened popup.
