# logging

Logging facilities for applications.

## Functions

### write

**Parameters:**

- `level`: `i32`
- `text_base`: `i32`
- `text_len`: `i32`

**Returns:** `none`

**Semantics:**

Writes the text starting from the memory address `text_base` with the length `text_len` to the environment-provided logger.

The text must be valid UTF-8 or otherwise the behavior is implementation-defined.

`level` can be one of:

- 1: Error
- 3: Warning
- 6: Info
