# Field Component

A set of components for building accessible form fields with labels, descriptions, and error messages.

## Components

- `FieldSet`: Container for multiple fields.
- `FieldGroup`: Container for grouping fields.
- `FieldLegend`: Legend for a fieldset.
- `Field`: Wrapper for a single field (label + input + description + error).
- `FieldLabel`: Label for the field.
- `FieldContent`: Wrapper for input/content.
- `FieldDescription`: Helper text.
- `FieldError`: Error message display.

## Usage

```tsx
import { Field, FieldLabel, FieldContent, FieldDescription, FieldError } from "@/components/ui/field"
import { Input } from "@/components/ui/input"

<Field>
  <FieldLabel>Username</FieldLabel>
  <FieldContent>
    <Input placeholder="Enter username" />
  </FieldContent>
  <FieldDescription>This is your public display name.</FieldDescription>
  <FieldError errors={[{ message: "Required" }]} />
</Field>
```

## Props

### Field
- `orientation`: "vertical" | "horizontal" | "responsive" (default: "vertical")

### FieldLegend
- `variant`: "legend" | "label" (default: "legend")

### FieldError
- `errors`: Array<{ message?: string } | undefined>