# Combobox Component

Autocomplete input and command palette with a list of suggestions.

## Components

- `Combobox`: Root.
- `ComboboxInput`: Input field with optional trigger/clear buttons.
- `ComboboxContent`: Dropdown content.
- `ComboboxList`: Scrollable list.
- `ComboboxItem`: Selectable item.
- `ComboboxEmpty`: Empty state.
- `ComboboxGroup`: Group of items.
- `ComboboxLabel`: Group label.
- `ComboboxChips`: Container for multi-select chips.
- `ComboboxChip`: Individual chip.

## Usage

```tsx
import { Combobox, ComboboxInput, ComboboxContent, ComboboxList, ComboboxItem, ComboboxEmpty } from "@/components/ui/combobox"

<Combobox>
  <ComboboxInput placeholder="Search..." />
  <ComboboxContent>
    <ComboboxList>
      <ComboboxEmpty>No results found.</ComboboxEmpty>
      <ComboboxItem value="1">Item 1</ComboboxItem>
      <ComboboxItem value="2">Item 2</ComboboxItem>
    </ComboboxList>
  </ComboboxContent>
</Combobox>
```

## Props

### ComboboxInput
- `showTrigger`: boolean (default: true)
- `showClear`: boolean (default: false)

### ComboboxChip
- `showRemove`: boolean (default: true)