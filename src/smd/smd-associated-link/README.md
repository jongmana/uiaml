# Associated Link

## Symbol
![image](smd-associated-link.png)

## Symbol Properties

| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Linktype | "L"\|"E" | Whether the link is triggered by a “click” from the user (in this case the indication “L” is optional) or by an event (“E”). |
| Link Id | String | A string that uniquely identifies the link in perspective of the contentarea the link originates from. |

## Documentation Properties
| Property | Type | Descriptionn|
|:----------:|:------:|-------------|
| Link Id | U*ia*ML path | Only required in case the trigger property will be described as well.<br> The path must identify the link symbol used within the diagram. |
| Trigger | String | In case the link is an event link, a description of what triggers the event is required. |

## Explanation
Like the common link the associated link is a link between a [contentarea](../smd-contentarea/README.md) and a [page](../smd-page/README.md). The difference with the [common link](../smd-link/README.md) is that the transition also triggers the content related to the associated link. This content is either visible but not visible within the current [Sitemap](../smd-sitemap/README.md), or offer the content to another system. That content is indicated by the dashed line, and the content is modeled outside the current [Sitemap symbol](../smd-sitemap/README.md) in order to show that is not something the user sees within the active content window.

Typical examples of such visible content related activities are [popups](../smd-popup/README.md), with triggers another [sitemap](../smd-sitemap/README.md) of the project we are modelling or the opening of a third party application like a mail client.
Writing the content on a file (for instance a .docx, .pdf or .xml) so that the file can be used by another system is an example of a non visible content related activity.<br>
Storing the content in a database is most of the time a system internal process, because the stored content is not meant to be leaving the project we are modeling via direct database access from a different system.
