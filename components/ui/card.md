# Card Component

A container component for displaying content in a box.

## Components

- `Card`: The main container.
- `CardHeader`: Header section.
- `CardTitle`: Title text.
- `CardDescription`: Description text.
- `CardContent`: Main content area.
- `CardFooter`: Footer section.
- `CardAction`: Action area (e.g. for buttons in the header).

## Usage

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

## Props

### Card
- `size`: "default" | "sm" (default: "default")
- `className`: string