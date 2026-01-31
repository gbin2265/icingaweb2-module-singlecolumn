# Single Column Dashboard Module for Icinga Web 2

This module provides an alternative dashboard layout where dashlets are displayed in a **single column** (stacked vertically) instead of the default multi-column grid layout.

## Features

- **Full-width dashlets**: Each dashlet takes 100% of the available width
- **Vertical stacking**: Dashlets are displayed one below another
- **Easy switching**: Quickly toggle between single column and grid view
- **All dashboards supported**: Works with all your existing dashboard panes
- **Responsive**: Works on all screen sizes
- **Print-friendly**: Better layout for printing dashboards

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
|           Dashlet4             |
+--------------------------------+
```

## Requirements

- Icinga Web 2 (>= 2.9.0)

## Installation

### Manual Installation

1. Extract the archive to your Icinga Web 2 modules directory:

```bash
tar -xzf singlecolumn-1.0.0.tar.gz -C /usr/share/icingaweb2/modules/
```

2. Enable the module:

```bash
icingacli module enable singlecolumn
```

Or enable via the web interface:
- Go to **Configuration** → **Modules**
- Find "singlecolumn" and click **Enable**

## Usage

After enabling the module, you can access the single column dashboard in two ways:

### Via Menu
1. Click on **Dashboard** in the main menu
2. Select **Single Column**

### Via URL
Navigate directly to: `https://your-icinga-server/icingaweb2/singlecolumn/dashboard`

### Switching Between Views

- When viewing the single column dashboard, click **"Grid View"** tab to return to the normal grid layout
- When viewing the normal dashboard, use the menu to access single column view

### Selecting Dashboard Panes

Just like the normal dashboard, you can switch between different panes using the tabs. All your existing dashboard panes are available in single column mode.

## Configuration

This module works out of the box with no configuration required. It uses your existing dashboard configuration from Icinga Web 2.

## License

This module is licensed under the GNU General Public License version 2 or later (GPLv2+).
