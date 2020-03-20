# Documentation Example

To import the repositories, a `docs` folder **must** be present! The repository won't be imported otherwise.

The main `docs` folder **must** contain a file called `_index.md` with the following content:

```
---
packageName: Name of the package
githubUrl: https://github.com/beyondcode/example
---
```

## Simple table of content

If the package does not require submenus, you can just place markdown files inside the `docs` folder.
Each markdown file needs a yaml front matter like the following:

```
---
title: Installation
order: 1
---

# Regular markdown content goes here

...
```

The `title` will be used within the menu and the HTML title attribute.
The `order` is used to sort the menu entries.

## Submenus

In order to create submenu structures in the documentation, create sub-folders inside the `docs` folder. Each subfolder that acts as a submenu **must** contain an `_index.md` file with the following content:

```
---
title: Getting Started
order: 0
---
```

This file is responsible of sorting the submenu and specify the submenu title.

Then place additional markdown files with the yaml front matter, just as you would within the docs root.