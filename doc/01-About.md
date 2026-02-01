# Single Column Dashboard Module

## About

The Single Column Dashboard module provides an alternative way to view your Icinga Web 2 dashboards. Instead of the default multi-column grid layout (2-3 columns depending on screen width), this module displays all dashlets in a single vertical column.

## Why Use Single Column?

- **Better readability**: Full-width dashlets show more information
- **Wide monitors**: Take advantage of ultra-wide displays
- **Presentations**: Better for displaying on TV screens or projectors

## How It Works

The module adds a new view (`/singlecolumn/dashboard`) that loads your existing dashboard configuration but displays dashlets at 100% width. No changes are made to your actual dashboard data.

## Navigation

- **URL**: `your-server/icingaweb2/singlecolumn/dashboard`
- **Tabs**: Use "Grid View" tab to switch back to normal layout

## Technical Details

- Module directory: `/usr/share/icingaweb2/modules/singlecolumn`
- Configuration: None required (uses existing dashboard config)
- CSS file: `public/css/singlecolumn.less`
