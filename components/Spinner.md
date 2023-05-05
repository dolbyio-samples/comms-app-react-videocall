# Spinner

The Spinner component is responsible for indicating loading states.

## Props

| Name                 | Type                    | Default       | Description                                               |
| -------------------- | ----------------------- | ------------- | --------------------------------------------------------- |
| `size` ?             | number                  | 32            | The size of the spinner width & height in px.             |
| `spinnerColor` ?     | ColorKey                | 'primary.400' | The color of the spinner.                                 |
| `textContent` ?      | string / number         | -             | The text displayed below the spinner.                     |
| `textContentColor` ? | ColorKey                | 'grey.100'    | The color of the text.                                    |
| `testID` ?           | string                  | -             | The unique E2E test handler.                              |
| `...HTMLDivElement`? | Partial(HTMLDivElement) | -             | Props that will be passed to the root of the div element. |

## Examples

### React

```javascript
return <Spinner textContent="Loading" />;
```
