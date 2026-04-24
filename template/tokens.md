Color tokens

$text-primary → #161616 (header text, icon color)
$text-secondary → #525252 (body cell text)
$layer-accent-01 → #e0e0e0 (thead background)
$layer-hover-01 → #e8e8e8 (row hover, overflow menu hover)
$layer-selected-01 → #d1d1d1 (selected row)
$border-subtle-00 → #f4f4f4 (td top border)
$border-subtle-01 → #c6c6c6 (td bottom border)
$link-primary → #0f62fe (resource name link)
$link-primary-hover → #0043ce
$focus → #0f62fe (selected row indicator / focus outline)
$background → #ffffff (table surface)


Spacing tokens

$spacing-03 → 8px (vertical breathing inside cells)
$spacing-05 → 16px (horizontal cell padding)


Type tokens

$heading-compact-01 → font-size: 14px; font-weight: 600; line-height: 1.28572; letter-spacing: 0.16px; (column headers)
$body-compact-01 → font-size: 14px; font-weight: 400; line-height: 1.28572; letter-spacing: 0.16px; (cells — note: computed got inflated to 16px by a parent rule but Carbon's intended token is $body-compact-01)
Font family: IBM Plex Sans


Size modifier

cds--data-table--md → header height 40px, row height 48px (47px rendered = 48px − 1px border)


Variants / flags

cds--data-table--visible-overflow-menu → forces the row overflow menu to be visible (not hover-only)


Motion tokens

Row hover transition uses $duration-fast-02 (~110ms) with $standard-easing (cubic-bezier(0.2, 0, 0.38, 0.9))