Variants observed / inferred in this instance:

Size modifier: cds--data-table--md (medium, 40px header / 48px rows). Carbon also supports xs (24px), sm (32px), lg (64px), xl (80px). Stacksync uses only md here.
Overflow-menu visibility: cds--data-table--visible-overflow-menu makes the per-row 3-dot menu button always visible instead of the Carbon default (visible only on row hover / focus).
Selectable rows: first column is a checkbox column (cds--table-column-checkbox) with a header-level "select all" checkbox and a per-row checkbox. This implies a "batch actions" toolbar appears elsewhere when rows are selected.
Row states

Default: transparent background, body text #525252.
Hover (inferred from Carbon): #e8e8e8 background, cursor pointer.
Selected (inferred from Carbon): #d1d1d1 background with 3px blue left indicator.
Focused row / cell: 2px blue #0f62fe outline.


Cell content variants observed:

Name: leading colored SVG icon (different icon per resource type — Workflow, Sync, Connection) + linked text in Carbon blue.
Apps: stacked 20×20 app logo images (Airtable, Snowflake, Salesforce, Zendesk, Shopify, GSheets, Python/Netsuite, Infinity/FellowSandbox).
Type: plain text (Workflow / Sync / Connection).
Status: Carbon Toggle (enabled = green #24a148; disabled = neutral). Rendered only for Sync/Workflow rows, absent for Connection rows.
Timestamps: <span class="min-w-[180px] line-clamp-1 break-all"> ensures min-width + truncation.
Overflow menu: ghost icon-only 3-dot button with tooltip.


Sticky header: the table is wrapped in .sticky-header-datatable-container, implying the <thead> remains fixed on vertical scroll.
Horizontal overflow: .cds--data-table-content wrapper enables horizontal scrolling on narrow viewports.