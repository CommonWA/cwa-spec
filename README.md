# Common WebAssembly API

## The project

Common WebAssembly API (CWA) is a minimal specification of a standard API to implement [non-Web WebAssembly](https://webassembly.org/docs/non-web/) in virtualized environments.

## Objectives

<sup>TODO: add how the project's objectives are inspired by WA official doc about "non-Web" WebAssembly ecosystem (with quotations)</sup>

## Structure

### Types

A few new types (which all lower to primitive WASM types) are introduced in `types.md`.

### Errors

Error handling in CWA is done by error codes, which are defined in `errors.md`.

### Namespaces

The CWA API is organized as *namespaces*, which each corresponds to a specific set of API functions.

CWA API functions should be accessible via the external module named `cwa`.

Every namespace should contain only lower-case ASCII characters in its name, and have its definitions in `ns/{namespace}.md`.

Every function should contain only lower-case ASCII characters, digits(0-9), and `_` in its name, and the first character cannot be a digit.

Functions from namespaces are visible to WebAssembly modules with the name `{namespace}_{function}`.

### URLs and Schemes

"Everything is a URL".

Defined in `urls-and-schemes.md`.

## Add new features to CWA

If you are not sure, open an issue to discuss your idea first.

After you've finished writing the definitions & explanations of your new namespaces/functions, open a pull request and we would be happy to review :-)
