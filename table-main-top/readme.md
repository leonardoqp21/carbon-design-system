ResourceSelect (Content Switcher)
What it does
A wrapper around the IBM Carbon Content Switcher component, used in Stacksync to filter the list of workspace resources by type (All Resources, Syncs, Workflows, Queues, Variables, Connections, API Proxies). It's a mutually-exclusive segmented control: only one tab can be active at a time, and switching it re-filters the resource table below.
When to use it

To toggle between filtered views of the same dataset when the options are few (2–7), share the same hierarchy, and don't require additional iconography.
Do NOT use when:

There are more than 7 options (prefer Dropdown or scrollable Tabs).
Multiple values need to be selected simultaneously (use checkboxes / multi-select).
Each section has its own complex content panel (use Carbon Tabs).

Implementation notes

The container uses role="tablist" and each item role="tab" with aria-selected kept in sync.
Expected keyboard navigation (Carbon spec): ←/→ move focus between tabs, Home/End jump to the first/last, Enter/Space activate.
Stacksync adds the utility class overflow-x-auto to the container to allow horizontal scrolling when there are many tabs on narrow viewports — recommended to keep in the design system as an optional modifier (resource-select--scrollable).
The black top/bottom borders on unselected items are intentional and, together, form the visual "outline" of the control (the container outline + the vertical borders on the buttons).