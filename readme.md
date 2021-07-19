# Lithium library

Check out the `repo/notes` branch for notes on repository specific branches and the repository as a whole.  
In this, the word "version" refers to any distinct release of the library, refered to by a semver (or any other versioning scheme).

## Project structure

### Branches
Basic branching structure

1.  Main branch (`main`)  
    This branch will contain only versions of lithium that compile and actually work. In other words, this branch should be **completely** stable.  
    The version referenced by this branch should be able to be exported and actually used in the real world.  
    The library may still be incomplete, but the only thing that matters is that at least the stuff that is there is actually stable and can maybe be used in real world stuff.  

2.  Development branch (`dev`)  
    Used for development of next version.  
    Can contain anything regardless of if it compiles or works. In other words, this branch can be unstable.  

### Tags

Tags can be used to document different versions/releases of the library. When using them in this manner, the tags should follow the **semver** format.  
When tagging unstable commits as versions (i.e. versions that cannot belong in main), mark them with the pre-release identifier `unstable`.  
When tagging a version that has documentation, mark it with the build identifier `documented`. It is alright for a snapshot of code to have two versions associated with it, one documented and another not documented.  

Version tag examples:
- `v0.1.0`
- `v6.3.2`
- `v2.6.4-unstable`
- `v2.6.4+documented`
- `v2.6.4-unstable+documented`
