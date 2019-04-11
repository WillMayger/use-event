# useEvent React Hook

This replaces the need for using `window.addEventListener()` when using react hooks.

You use it in exactly the same way as `window.addEventListener()`.

## Install

Yarn:
`yarn add use-add-event`

NPM:
`npm install --save use-add-event`

## Usage

`useEvent(event, handler, useCapture)`

event: STRING - any event listener event as a string.
handler: FUNCTION - function to be called when the event is triggered.
useCapture: BOOL - determining passive event or not (defaults to false).

Example:
```
import useEvent from 'use-add-event';

export default function MyComponent() {
  const handleResize = (e) => { ... };
  useEvent('resize', handleResize);
  return (
    ...
  )
}
```
