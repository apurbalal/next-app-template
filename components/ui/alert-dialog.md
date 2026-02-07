# AlertDialog Component

A modal dialog that interrupts the user with important content and expects a response.

## Components

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

## Usage

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

## Props

### AlertDialogContent
- `size`: "default" | "sm" (default: "default")