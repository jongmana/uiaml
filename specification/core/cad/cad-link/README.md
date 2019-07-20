# Link

## Symbol
![image](cad-link.png)

## Symbol Properties

| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Linktype | "L"\|"E" | Whether the link is triggered by a “click” from the user (in this case the indication “L” is optional) or by an event (“E”). |
| Link Id | String | A string that corresponds to the [Link Id](../../smd/smd-link/README.md) of the outgoing links of this contentarea as modelled within the Sitemap Diagram (SMD).

## Documentation Properties
| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| - | - | - |

## Explanation
The Link Id's used within the CAD must match those used within the SMD. Within the CAD the link source of a normal link (linktype “L”) must be a CAE, indicated by placing the start point of the link within the CAE that triggers the link. The link destination is pointing somewhere outside the [contentarea element](../cad-contentarea/README.md).
In case the link is an event link, the start point of the link is the frame of the contentarea element itself.
Within the CAD there may be more than one link with the same Link Id. They however represent a single link with the same Link Id in the SMD.
