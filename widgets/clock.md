---
title: Clock Widget
order: 1
---

# Clock Widget

The Clock widget displays the current time and date.

## Features

- Digital or analog display
- Multiple timezone support
- Customizable date format
- 12/24 hour format

## Configuration

| Option | Description | Default |
|--------|-------------|---------|
| `format` | Time format (12h/24h) | `24h` |
| `showDate` | Display date | `true` |
| `showSeconds` | Display seconds | `false` |
| `timezone` | Timezone | System default |
| `style` | Display style (digital/analog) | `digital` |

## Examples

### Basic Clock

```json
{
  "type": "clock",
  "config": {
    "format": "24h",
    "showDate": true
  }
}
```

### World Clock

Show multiple timezones:

```json
{
  "type": "clock",
  "config": {
    "timezone": "America/New_York",
    "label": "New York"
  }
}
```

## Styling

The clock inherits your theme colors. Custom CSS classes:

- `.widget-clock` - Main container
- `.clock-time` - Time display
- `.clock-date` - Date display
