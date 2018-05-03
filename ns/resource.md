# resource

Operations related to readable/writeable resources.

## Functions

### resource_read

**Parameters:**

- `id`: `i32`
- `data`: `&mut [u8]`

**Returns:** `i32`

**Semantics:**

Reads from the resource specified by `id`, into `data`.

Returns the actual bytes read on success, or the error on failure.

### resource_write

**Parameters:**

- `id`: `i32`
- `data`: `&[u8]`

**Returns:** `i32`

**Semantics:**

Writes `data` to the resource specified by `id`.

Returns the actual bytes written on success, or the error on failure.

### resource_close

**Parameters:**

- `id`: `i32`

**Returns:** `none`

**Semantics:**

Closes the resource specified by `id`.

Calling this on an invalid resource id is a fatal error.
