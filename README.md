# Single Column Dashboard Module for Icinga Web 2

This module provides an alternative dashboard layout where dashlets are displayed in a **single column** (stacked vertically) instead of the default multi-column grid layout.

## Features

- **Full-width dashlets**: Each dashlet takes 100% of the available width
- **Vertical stacking**: Dashlets are displayed one below another
- **All dashboards supported**: Works with all your existing dashboard panes
- **Identical styling**: Same look and feel as standard Icinga Web 2, only wider

## Layout Comparison

### Default Grid Layout (3 columns)
```
+----------+----------+----------+
| Dashlet1 | Dashlet2 | Dashlet3 |
+----------+----------+----------+
| Dashlet4 | Dashlet5 | Dashlet6 |
+----------+----------+----------+
```

### Single Column Layout
```
+--------------------------------+
|           Dashlet1             |
+--------------------------------+
|           Dashlet2             |
+--------------------------------+
|           Dashlet3             |
+--------------------------------+
```

## Requirements

- Icinga Web 2 (>= 2.9.0)

## Installation

1. Extract the archive to your Icinga Web 2 modules directory:

```bash
tar -xzf singlecolumn-1.0.0.tar.gz -C /usr/share/icingaweb2/modules/
```

2. Enable the module:

```bash
icingacli module enable singlecolumn
```

Or enable via the web interface: **Configuration** → **Modules** → **singlecolumn** → **Enable**

## Usage

Navigate to the single column dashboard via URL:

```
https://your-icinga-server/icingaweb2/singlecolumn/dashboard
```

To select a specific pane, add the `pane` parameter:

```
https://your-icinga-server/icingaweb2/singlecolumn/dashboard?pane=Current%20Incidents
```

Use the **Grid View** tab to switch back to the normal multi-column layout.

## Configuration

No configuration required. The module uses your existing dashboard configuration.

## License

GPLv2+
