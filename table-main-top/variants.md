Variants observed / inferred on screen:

Size: only md is detected (cds--content-switcher--md, 36px height). Carbon also exposes sm (32px) and lg (48px), but they are not in use here.
Button state

Selected (cds--content-switcher--selected + aria-selected="true" + tabindex="0"): #161616 background, white text, rounded corners only if it's the first or last item.
Unselected (aria-selected="false" + tabindex="-1"): transparent background, #525252 text, black top/bottom borders.
Hover (on unselected): #e8e8e8 background.
Focus: blue #0f62fe outline, -2px offset.
Disabled (inferred, not present on screen): #c6c6c6 text and borders, not-allowed cursor.


Overflow: the container has overflow-x-auto added by Stacksync. With many tabs (All Resources / Syncs / Workflows / Queues / Variables / Connections / API Proxies) it enables horizontal scrolling on narrow viewports.
Layout constraints: responds to Carbon's Layout system — default size md, minimum sm, maximum lg.
Item count: 7 tabs visible in this extraction (All Resources, Syncs, Workflows, Queues, Variables, Connections, API Proxies). The component is agnostic to the number of items.