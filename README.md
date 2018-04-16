# Metal

Metal is a minimal specification of the standard API for non-Web WebAssembly usermode environments.

## Structure

The Metal API is organized as *namespaces*, which each corresponds to a specific set of API functions.

Every namespace should contain only lower-case ASCII characters in its name, and have its definitions in `ns/{namespace}.md`.

Every function should contain only lower-case ASCII characters, digits(0-9), and `_` in its name, and the first character cannot be a digit.

Functions from namespaces are visible to WebAssembly modules with the name `__metal_{namespace}_{function}`.

## Add new features to Metal

If you are not sure, open an issue to discuss your idea first.

After you've finished writing the definitions & explanations of your new namespaces/functions, open a pull request and we would be happy to review :-)
