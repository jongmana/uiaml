# Contentarea

## Symbol
![image](smd-contentarea.png)

## Symbol Properties

| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Contentarea Id | String | Unique name within the site project for each content grouping. |

## Documentation Properties
| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Contentarea Id | U*ia*ML path | The Contentarea Id part of the U*ia*ML path has to be identical to the one used by the Symbol property.|
| Description | String | Text that describes the information that will be represenated by this contentarea. |

## Explanation
A contentarea is the container that hold several contentarea elements (CAE), like text, images or input fields. There are no hard rules about the boundaries of a contentarea, but often a deployed contentarea is recognizable by a different background or a frame that groups the content.
A contentarea might reappear on several different pages within a single site. The menu is an example of such a contentarea.
Within a U*ia*ML Sitemap there is for each contentarea with the same contentarea Id exactly one contentarea symbol in which the contentarea Id is underlined. This is the defining contentarea. Only from that contentarea [links](../smd-link/README.md) to other [pages](../smd-page/README.md) may be drawn.
