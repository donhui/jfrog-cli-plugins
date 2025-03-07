# rm-empty

## About this plugin
This plugin can help find out the most popularly downlaoded artifacts in a given repository, Artifacts that are consuming the most space in a given repository with various levels of customization avaialble. Results obtained can also be sorted and filtered.

## Installation with JFrog CLI
Installing the latest version:

`$ jfrog plugin install rm-empty`

Installing a specific version:

`$ jfrog plugin install rm-empty@version`

Uninstalling a plugin

`$ jfrog plugin uninstall rm-empty`

## Usage
### Commands
* folders 
    - Arguments:
        - path - A path in Artifactory, under which to remove all the empty folders.
    - Flags:
        - server-id: The JFrog instance ID configured using the ```jfrog c add``` command. If not provided, the default configured instance is used.
        - quiet: Skip the delete confirmation message
    - Examples:
    ```
    $ jfrog rm-empty folders repository/path/in/rt/

    $ jfrog rm-empty folders repository/path/in/rt/ --quiet

    $ jfrog rm-empty f repository/path/in/rt/

    $ jfrog rm-empty f repository/path/in/rt/ --server-id my-server-id
    ```

### Environment variables
None.

## Additional info
None.

## Release Notes
The release notes are available [here](RELEASE.md).
