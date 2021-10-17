# Python Packaging Index (PyPI)

PyPI is the default home for package management on Python. It is run by the Python Software Foundation, and can be accessed by developers via the `pip` client.

## Yanking or Deletion of Versions

The Python Packaging Index allows _owners_ of packages to delete files, releases, and the entire project itself. PyPI also presents a "yank" mechanism for releases. Yanked releases are ignored by installers unless the version is explicitly declared by a dependent package.

## Deletion of Projects / Potential for Squatting

PyPI also doesn't allow the *file names* to be reused. However, if a project is deleted, the project name can be reused by a different account. In this instance, changing the version number is enough to change the file name of the package. This was tested by deleting a test project off one account, and reuploading on another. A version change was sufficient for the second account to own the project name.

The formal guidelines for managing situations of name squatting and the takeover of abandoned packages are laid out in PEP-541.

## Sources

1. Yanked releases: https://pypi.org/help/#yanked, archived at https://archive.is/ltgJl
2. File name reuse: https://pypi.org/help/#file-name-reuse, archived at https://archive.is/ltgJl
3. Collaborator roles: https://pypi.org/help/#collaborator-roles, archived at https://archive.is/ltgJl
4. PEP-541: https://www.python.org/dev/peps/pep-0541/
