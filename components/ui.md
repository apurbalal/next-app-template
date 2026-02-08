# UI Components

This document provides an overview of the available UI components, their sub-components, usage examples, and props.

## Alert Dialog

A modal dialog that interrupts the user with important content and expects a response.

### Components
- `AlertDialog`: Root.
- `AlertDialogTrigger`: Trigger.
- `AlertDialogContent`: Content.
- `AlertDialogHeader`: Header.
- `AlertDialogTitle`: Title.
- `AlertDialogDescription`: Description.
- `AlertDialogFooter`: Footer.
- `AlertDialogAction`: Confirm action.
- `AlertDialogCancel`: Cancel action.
- `AlertDialogMedia`: Media area (icon/image).

### Usage
```tsx
import { AlertDialog, AlertDialogTrigger, AlertDialogContent, AlertDialogHeader, AlertDialogTitle, AlertDialogDescription, AlertDialogFooter, AlertDialogAction, AlertDialogCancel } from "@/components/ui/alert-dialog"

<AlertDialog>
  <AlertDialogTrigger>Open</AlertDialogTrigger>
  <AlertDialogContent>
    <AlertDialogHeader>
      <AlertDialogTitle>Are you sure?</AlertDialogTitle>
      <AlertDialogDescription>This action cannot be undone.</AlertDialogDescription>
    </AlertDialogHeader>
    <AlertDialogFooter>
      <AlertDialogCancel>Cancel</AlertDialogCancel>
      <AlertDialogAction>Continue</AlertDialogAction>
    </AlertDialogFooter>
  </AlertDialogContent>
</AlertDialog>
```

### Props
**AlertDialogContent**
- `size`: "default" | "sm" (default: "default")

---

## Badge

Displays a badge or a component that looks like a badge.

### Usage
```tsx
import { Badge } from "@/components/ui/badge"

<Badge variant="default">Badge</Badge>
```

### Props
**Badge**
- `variant`: "default" | "secondary" | "destructive" | "outline" | "ghost" | "link" (default: "default")

---

## Button

Displays a button or a component that looks like a button.

### Usage
```tsx
import { Button } from "@/components/ui/button"

<Button variant="default" size="default">Click me</Button>
```

### Props
**Button**
- `variant`: "default" | "outline" | "secondary" | "ghost" | "destructive" | "link" (default: "default")
- `size`: "default" | "xs" | "sm" | "lg" | "icon" | "icon-xs" | "icon-sm" | "icon-lg" (default: "default")
- `asChild`: boolean (default: false)

---

## Card

A container component for displaying content in a box.

### Components
- `Card`: The main container.
- `CardHeader`: Header section.
- `CardTitle`: Title text.
- `CardDescription`: Description text.
- `CardContent`: Main content area.
- `CardFooter`: Footer section.
- `CardAction`: Action area.

### Usage
```tsx
import { Card, CardHeader, CardTitle, CardDescription, CardContent, CardFooter } from "@/components/ui/card"

<Card size="default">
  <CardHeader>
    <CardTitle>Title</CardTitle>
    <CardDescription>Description</CardDescription>
  </CardHeader>
  <CardContent>
    Content
  </CardContent>
  <CardFooter>
    Footer
  </CardFooter>
</Card>
```

### Props
**Card**
- `size`: "default" | "sm" (default: "default")
- `className`: string

---

## Dropdown Menu

Displays a menu to the user—such as a set of actions or functions—triggered by a button.

### Components
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

### Usage
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

### Props
**DropdownMenuContent**
- `align`: "start" | "center" | "end" (default: "start")
- `sideOffset`: number (default: 4)

**DropdownMenuItem**
- `inset`: boolean
- `variant`: "default" | "destructive"

---

## Field

A set of components for building accessible form fields with labels, descriptions, and error messages.

### Components
- `FieldSet`: Container for multiple fields.
- `FieldGroup`: Container for grouping fields.
- `FieldLegend`: Legend for a fieldset.
- `Field`: Wrapper for a single field.
- `FieldLabel`: Label for the field.
- `FieldContent`: Wrapper for input/content.
- `FieldDescription`: Helper text.
- `FieldError`: Error message display.

### Usage
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

### Props
**Field**
- `orientation`: "vertical" | "horizontal" | "responsive" (default: "vertical")

**FieldLegend**
- `variant`: "legend" | "label" (default: "legend")

**FieldError**
- `errors`: Array<{ message?: string } | undefined>

---

## Input

Displays a form input field or a component that looks like an input field.

### Usage
```tsx
import { Input } from "@/components/ui/input"

<Input type="email" placeholder="Email" />
```

---

## Input Group

A composable component for creating complex input layouts with addons and buttons.

### Components
- `InputGroup`: Container.
- `InputGroupAddon`: Wrapper for addons.
- `InputGroupButton`: Button inside the group.
- `InputGroupText`: Text addon.
- `InputGroupInput`: Input field.
- `InputGroupTextarea`: Textarea field.

### Usage
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

### Props
**InputGroupAddon**
- `align`: "inline-start" | "inline-end" | "block-start" | "block-end" (default: "inline-start")

**InputGroupButton**
- `size`: "xs" | "sm" | "icon-xs" | "icon-sm" (default: "xs")
- `variant`: Button variants (default: "ghost")

---

## Label

Renders an accessible label associated with controls.

### Usage
```tsx
import { Label } from "@/components/ui/label"

<Label htmlFor="email">Email</Label>
```

---

## Select

Displays a list of options for the user to pick from—triggered by a button.

### Components
- `Select`: Root.
- `SelectTrigger`: Trigger button.
- `SelectValue`: Value display.
- `SelectContent`: Dropdown content.
- `SelectItem`: Option item.
- `SelectGroup`: Group of items.
- `SelectLabel`: Group label.
- `SelectSeparator`: Separator.

### Usage
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

### Props
**SelectTrigger**
- `size`: "default" | "sm" (default: "default")

**SelectContent**
- `position`: "item-aligned" | "popper" (default: "item-aligned")

---

## Separator

Visually or semantically separates content.

### Usage
```tsx
import { Separator } from "@/components/ui/separator"

<Separator orientation="horizontal" />
```

### Props
**Separator**
- `orientation`: "horizontal" | "vertical" (default: "horizontal")
- `decorative`: boolean (default: true)

---

## Textarea

Displays a form textarea.

### Usage
```tsx
import { Textarea } from "@/components/ui/textarea"

<Textarea placeholder="Type your message here." />
```
