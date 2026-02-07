# InputGroup Component

A composable component for creating complex input layouts with addons and buttons.

## Components

- `InputGroup`: Container.
- `InputGroupAddon`: Wrapper for addons (text, buttons, icons).
- `InputGroupButton`: Button inside the group.
- `InputGroupText`: Text addon.
- `InputGroupInput`: Input field.
- `InputGroupTextarea`: Textarea field.

## Usage

```tsx
import { InputGroup, InputGroupAddon, InputGroupText, InputGroupInput } from "@/components/ui/input-group"
import { Search } from "lucide-react"

<InputGroup>
  <InputGroupAddon>
    <Search />
  </InputGroupAddon>
  <InputGroupInput placeholder="Search..." />
  <InputGroupAddon align="inline-end">
    <InputGroupText>Cmd+K</InputGroupText>
  </InputGroupAddon>
</InputGroup>
```

## Props

### InputGroupAddon
- `align`: "inline-start" | "inline-end" | "block-start" | "block-end" (default: "inline-start")

### InputGroupButton
- `size`: "xs" | "sm" | "icon-xs" | "icon-sm" (default: "xs")
- `variant`: Button variants (default: "ghost")