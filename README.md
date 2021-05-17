# Generating this example

Run generate.js from the directory you have cloned node-static-sites into.

Example:

    node ../node_static_sites/generate.js

This example assumes that node-static-sites was cloned into the directory
`node_static_sites` next to the current directory.

On Windows:

node ..\node_static_sites\generate.js

# Caveat about this example

This example uses the implicitly available value `pageRootPath` to resolve resources.

The reason for this is that the example's output is supposed to work from the file system, as opposed to a web server.

For real applications, please attempt to avoid using `pageRootPath`, and instead use `/` or a root path for your deployment situation, which you can configure in `globals.json`.
