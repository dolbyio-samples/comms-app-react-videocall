# useErrors

The useErrors hook expose errors and methods to remove handled ones.

## Members

| Name                  | Type                            | Description                                                                     |
| --------------------- | ------------------------------- | ------------------------------------------------------------------------------- |
| `sdkErrors`           | ErrorsType['sdkErrors']         | Errors related to sdk (connection , sessions, tokens).                          |
| `screenShareErrors`   | ErrorsType['screenShareErrors'] | Errors related to screen sharing.                                               |
| `recordingErrors`     | ErrorsType['recordingErrors']   | Errors related to videocall recording.                                          |
| `removeSdkErrors`     | (error?: ErrorCodes) => void    | Remove specific error or clean sdk errors.                                      |
| `setErrorsExplicitly` | (params? ErrorParams) => void   | Sets specific error. Also can be used for exception purposes inside application |

## Examples

### React

### Remove specific error from sdk errors

```javascript
const { removeSdkErrors } = useMessage();

removeSdkErrors(ErrorCode.IncorrectSession);
```

### Simulate error/ set specific error

```javascript
const { setErrorsExplicitly } = useMessage();
setErrorsExplicitly({ error: ErrorCodes.IncorrectSession, context: 'sdkErrors' });
```
