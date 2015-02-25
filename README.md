# Skin Installer for Roundcube

This installer ensures that skins end up in the correct directory:

 * `<roundcube-root>/skins/skin-name`

## Minimum setup

 * create a `composer.json` file in your skin's repository
 * add the following contents

### sample composer.json for plugins

    {
        "name": "yourvendor/skin-name",
        "license": "the license",
        "description": "describe your skin",
        "type": "roundcube-skin",
        "authors": [
            {
                "name": "<your-name>",
                "email": "<your-email>"
            }
        ],
        "require": {
            "lucasmarin/skin-installer": "*"
        },
        "minimum-stability": "dev-master"
    }

## Installation

 * clone Roundcube
 * `cp composer.json-dist composer.json`
 * add your plugin in the `require` section of composer.json
 * `composer.phar install`
