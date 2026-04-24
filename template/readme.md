ResourceDataTable (Carbon DataTable)
What it does
A wrapper around IBM Carbon's DataTable used in Stacksync to list every resource in a workspace (Syncs, Workflows, Queues, Variables, Connections, API Proxies). Each row represents a single resource with its identifying icon, name link, connected apps, type, enable/disable toggle, creation timestamp, last-modified timestamp, and an overflow menu with per-row actions.
When to use it

Displaying large tabular datasets with consistent column semantics where users need to scan, sort, filter, select, and act on rows.
Pairs naturally with the ResourceSelect content switcher (previous component) and a toolbar containing search + region filter.
Do NOT use when:

The dataset is a small list of simple items (prefer StructuredList or a plain list).
Items are card-like and visual hierarchy matters more than tabular comparison (prefer a grid of Tile / Card).
Rows are strictly read-only and very numerous (consider virtualized rendering).
Implementation notes

The component combines several Carbon primitives: DataTable, Checkbox, OverflowMenu, Toggle, Tooltip. Keep it composable by letting consumers inject cell renderers.
The sticky-header wrapper is a Stacksync addition (sticky-header-datatable-container). Re-implement with position: sticky; top: 0; z-index: 1; on the <thead> cells and make sure the wrapper has a defined max-height for the effect to work.
cds--data-table--visible-overflow-menu is a Stacksync/Carbon flag that toggles the default "icon appears only on row hover" behavior — make it a boolean prop, not a styling override.
Accessibility: <th scope="col"> on every header, aria-live="off" on the select-all header cell (so announcing row selections doesn't spam screen readers), and visually-hidden labels on checkboxes.
Keyboard support expected (Carbon spec): Tab through cells with interactive content, Space to toggle checkboxes, Enter / Space to open the overflow menu, Esc to close it.
Cells with timestamps use Tailwind-style utilities (min-w-[180px] line-clamp-1 break-all) to guarantee a minimum column width and truncate overflow — worth standardizing as a dedicated DataTableCell--truncate modifier in the design system.