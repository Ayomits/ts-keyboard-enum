# ts-keyboard-enum
I've created this library, because `event.code` in default `KeyboardEvent` is not type-safe

You can use for check like this:
```ts
useKeyboardShortcut(
    ev => ev.ctrlKey && ev.code === KeyboardKeys.KeyK,
    () => {
      setIsSearchOpen(prev => !prev);
      if (!isSearchOpen === true) {
        desktopInputRef.current?.focus();
      }
    }
  );
```

This react hook you can use in my other library `use-keydown-keyboard-shortcut`
