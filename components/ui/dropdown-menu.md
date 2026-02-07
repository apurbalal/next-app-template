# DropdownMenu Component

Displays a menu to the user—such as a set of actions or functions—triggered by a button.

## Components

- `DropdownMenu`: Root.
- `DropdownMenuTrigger`: Trigger element.
- `DropdownMenuContent`: The menu content.
- `DropdownMenuItem`: Action item.
- `DropdownMenuCheckboxItem`: Checkbox item.
- `DropdownMenuRadioGroup`: Radio group.
- `DropdownMenuRadioItem`: Radio item.
- `DropdownMenuLabel`: Label.
- `DropdownMenuSeparator`: Separator.
- `DropdownMenuShortcut`: Keyboard shortcut display.
- `DropdownMenuSub`: Submenu root.
- `DropdownMenuSubTrigger`: Submenu trigger.
- `DropdownMenuSubContent`: Submenu content.

## Usage

```tsx
import { DropdownMenu, DropdownMenuTrigger, DropdownMenuContent, DropdownMenuItem } from "@/components/ui/dropdown-menu"

<DropdownMenu>
  <DropdownMenuTrigger>Open</DropdownMenuTrigger>
  <DropdownMenuContent>
    <DropdownMenuItem>Item 1</DropdownMenuItem>
    <DropdownMenuItem>Item 2</DropdownMenuItem>
  </DropdownMenuContent>
</DropdownMenu>
```

## Props

### DropdownMenuContent
- `align`: "start" | "center" | "end" (default: "start")
- `sideOffset`: number (default: 4)

### DropdownMenuItem
- `inset`: boolean
- `variant`: "default" | "destructive"