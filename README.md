# Odoo Snippets for Zed

<p align="center">
  <img src="https://raw.githubusercontent.com/droggol/VscOdooSnippets/master/images/icon.png" alt="Odoo Snippets logo" width="128" height="128"/>
</p>

This repository now ships the Odoo snippet collection originally created for VS Code by the [Droggol/VscOdooSnippets](https://github.com/Droggol/VscOdooSnippets) project.

Each package targets a specific file type while following the official [Odoo Guidelines](https://www.odoo.com/documentation/15.0/reference/guidelines.html) and works out of the box in the [Zed](https://zed.dev) editor.

## Features
- Fast boilerplate for common Odoo ORM patterns, fields, and CRUD overrides.
- XML scaffolding for menus, views, actions, reports, assets, and QWeb templates.
- JavaScript/OWL lifecycle helpers, state hooks, and module headers.
- CSV templates for access control lists and data imports.

## Installation (Zed)
1. Copy or symlink the desired language folder (for example `odoo-snippets/`) into your Zed extensions directory (typically `~/.config/zed/extensions/`).
2. Launch Zed and run `Extensions: Reload` (command palette) or restart the editor.
3. Open an Odoo project file; start typing a prefix such as `oomodel` (Python) or `<form` (XML) and accept the snippet from completions.

## Searching snippets
- Use Zed’s completion menu: type the prefix and confirm with `Tab`/`Enter`.
- Browse the snippet files under `<extension>/snippets/**.json` to see the raw bodies.
- The tables below mirror the upstream documentation for quick lookup.

## Python snippets (`.py`)

| Prefix | Purpose |
| --- | --- |
| `manifest` | Manifest JSON |
| `imo` | Import Odoo Model/Fields/API |
| `ime` | Import Odoo Exceptions |
| `iml` | Import Logging |
| `imf` | Import From |
| `oomodel` | Add model |
| `oofchar` | Char Field |
| `ooftext` | Text Field |
| `oofhtml` | Html Field |
| `oofboolean` | Boolean Field |
| `oofinteger` | Integer Field |
| `ooffloat` | Float Field |
| `oofselection` | Selection Field |
| `oofdate` | Date Field |
| `oofdatetime` | Datetime Field |
| `oofimage` | Image Field |
| `oofbinary` | Binary Field |
| `oofmonetary` | Monetary Field |
| `oofmany2one` | Many2one Field |
| `oofone2many` | One2many Field |
| `oofmany2many` | Many2many Field |
| `oofcompute` | Compute Field |
| `oofcomputei` | Compute Field with Inverse |
| `oofonchange` | Onchange Field |
| `oofconstrains` | Field Constrains |
| `oofconstrains` | SQL Constraints |
| `ooone` | Ensure One |
| `oooverride` | Override Method |
| `oocreate` | Create Method |
| `oowrite` | Write Method |
| `oounlink` | Unlink Method |
| `related` | Related Attribute |
| `required` | Required Attribute |
| `readonly` | Readonly Attribute |
| `copy` | Copy Attribute |
| `store` | Store Attribute |
| `digits` | Digits Attribute |
| `help` | Help Attribute |
| `check_company` | Check Company Attribute |
| `ooleaf` | Domain Leaf |

## XML snippets (`.xml`)

| Prefix | Purpose |
| --- | --- |
| `<odoo>` | Odoo Namespace |
| `<data>` | Data Tag |
| `<menuitem>` | Root Menu |
| `<menuitem>` | Submenu |
| `<form>` | Form View |
| `<tree>` | Tree View |
| `<list>` | List View |
| `<kanban>` | Kanban View |
| `<search>` | Search View |
| `<calendar>` | Calendar View |
| `<cohort>` | Cohort View |
| `<gantt>` | Gantt View |
| `<graph>` | Graph View |
| `<pivot>` | Pivot View |
| `<activity>` | Activity View |
| `<qweb>` | Qweb View |
| `<viewInherit>` | Inherit View |
| `<buttonHeader>` | Button in Form View Header |
| `<buttonBox>` | Stat Button Container |
| `<buttonStat>` | Stat Button |
| `<field>` | Self Closing Field |
| `<field>` | Field |
| `<filter>` | Filter in Search View |
| `<notebook>` | Notebook |
| `<page>` | Notebook Page |
| `<chatter>` | Chatter |
| `<action>` | Action |
| `<actionView>` | View in Action |
| `<actionServer>` | Server Action |
| `<actionUrl>` | URL Action |
| `<actionClient>` | Client Action |
| `<actionReport>` | Report Action |
| `<report>` | Report Template |
| `<cron>` | Cron |
| `<ir_model>` | Define a new ir.model entry |
| `<ir_field>` | Create an ir.model.fields record |
| `<ir_default_field>` | Set a default value via ir.default |
| `<ir_field_m2o>` | Define a many2one ir.model.fields entry |
| `<ir_field_m2m>` | Define a many2many ir.model.fields entry |
| `<ir_field_o2m>` | Define a one2many ir.model.fields entry |
| `<ir_field_computed>` | Computed field with depends and code |
| `<ir_field_related>` | Related field definition |
| `<ir_action_server>` | Server action executing Python code |
| `<base_automation>` | Base automation rule triggering a server action |
| `<ir_action_server_controller>` | Server action exposed as website controller |
| `<record>` | Record |
| `<function>` | Function |
| `<template>` | Template |
| `<templateInherit>` | Inherit Template |
| `<xpath>` | Xpath |
| `<xpathAttr>` | Xpath to Attributes |
| `<xpathField>` | Xpath for Field |
| `<attribute>` | Attribute for Xpath |
| `<group>` | Group |
| `<script>` | Script |
| `<link>` | SCSS Link |
| `<assetsBackend>` | Backend Assets |
| `<assetsFrontend>` | Frontend Assets |
| `<t-if>` | Evaluate node when python expression is truthy |
| `<t-if-else>` | If/elif/else structure |
| `<t-elif>` | Switched branch for preceding t-if |
| `<t-else>` | Fallback branch for preceding t-if |
| `<t-foreach>` | Loop over a collection and expose helpers |
| `t-as` | Name the loop variable (use with t-foreach) |
| `t-groups` | Restrict rendering to users in (or outside with !) a group |
| `groups` | Alias for t-groups |
| `t-options` | Configure directives like t-call, t-field or t-out |
| `t-options-` | Add a key to the __qweb_options__ dict |
| `<t-set>` | Assign an expression result into values[name] |
| `<t-set-block>` | Capture rendered body into values[name] |
| `t-value` | Expression used with t-set |
| `t-valuef` | Format string expression used with t-set |
| `<t-out>` | Output value or fallback content when falsy |
| `<t-field>` | Render a model field with optional default content |
| `<t-esc>` | Deprecated alias for t-out |
| `<t-raw>` | Deprecated alias for t-out (unsafe HTML) |
| `<t-call>` | Render another template with an isolated context |
| `<t-call-assets>` | Serve asset bundles returned by _get_asset_nodes |
| `t-lang` | Render the t-call target in another language |
| `<t-debug>` | Breakpoint (empty uses PYTHONBREAKPOINT) |
| `<t-log>` | Log expression evaluation to server logs |
| `t-att` | Populate __qweb_attrs__ with python expressions |
| `t-attf` | Format string version of t-att |
| `t-att=` | Assign dict of attributes via t-att |
| `t-qweb-skip` | Skip rendering and directives for current node |
| `t-tag-open` | Technical directive: emit opening tag |
| `t-tag-close` | Technical directive: emit closing tag |
| `<t-inner-content>` | Technical directive: render child nodes |
| `<t-consumed-options>` | Validate that t-options keys got consumed |
| `t-else-valid` | Technical marker for valid else branch |
| `ooleaf` | Domain Leaf |

## JavaScript snippets (`.js`)

| Prefix | Purpose |
| --- | --- |
| `odoo-module` | Define Odoo Module |
| `imc` | Import Component |
| `imcs` | Import Component and useState |
| `oc` | Component |
| `occ` | Component with Constructor |
| `ocs` | Component with Setup |
| `ms` | Setup |
| `mws` | willStart |
| `mm` | mounted |
| `mwup` | willUpdateProps |
| `mwp` | willPatch |
| `mp` | patched |
| `mwum` | willUnmount |
| `mce` | catchError |
| `uss` | useState |
| `usr` | useRef |
| `usc` | useContext |
| `ust` | useStore |
| `usd` | useDispatch |
| `onm` | onMounted |
| `onwum` | onWillUnmount |
| `onwp` | onWillPatch |
| `onp` | onPatched |
| `onws` | onWillStart |
| `onwup` | onWillUpdateProps |

Hooks and lifecycle snippets include the method bodies from the original VS Code extension; insert them inside your OWL components as needed.

## CSV snippets (`.csv`)

| Prefix | Purpose |
| --- | --- |
| `oocolumns` | Columns |
| `ooaccess` | Access for All Groups |
| `ooaccess` | Access for Specific Group |

## Contributing
- Issues and PRs specific to this Zed port are welcome in this repository.
- Snippet logic originates from Droggol’s project; for upstream improvements, consider contributing there as well.

## Credits
- Original snippets by [Droggol](https://github.com/Droggol/VscOdooSnippets)
