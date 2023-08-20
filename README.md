# IDEA-328273 reproducer

this project has a Maven submodule as well as a python submodule.

since the python submodule would have no configured interpreter by default,
we have to craft an `.iml` file for it.

Ideally, the module would still
be discovered and automatically imported.
However, for now, it requires an extra step:
right-clicking on the .iml file,
and then selecting `import` from the context menu.
