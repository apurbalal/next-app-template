# Select Component

Displays a list of options for the user to pick from—triggered by a button.

## Components

- `Select`: Root.
- `SelectTrigger`: Trigger button.
- `SelectValue`: Value display.
- `SelectContent`: Dropdown content.
- `SelectItem`: Option item.
- `SelectGroup`: Group of items.
- `SelectLabel`: Group label.
- `SelectSeparator`: Separator.

## Usage

```tsx
import { Select, SelectTrigger, SelectValue, SelectContent, SelectItem } from "@/components/ui/select"

<Select>
  <SelectTrigger>
    <SelectValue placeholder="Select an option" />
  </SelectTrigger>
  <SelectContent>
    <SelectItem value="1">Option 1</SelectItem>
    <SelectItem value="2">Option 2</SelectItem>
  </SelectContent>
</Select>
```

## Props

### SelectTrigger
- `size`: "default" | "sm" (default: "default")

### SelectContent
- `position`: "item-aligned" | "popper" (default: "item-aligned")