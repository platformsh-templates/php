> [!WARNING]
> **This repository is no longer maintained by our internal teams.**  
> The template is provided *as is* and will not receive updates, bug fixes, or new features.  
> You are welcome to contribute on it or fork the repository and modify it for your own use.
> To deploy this template on [Upsun](https://www.upsun.com), you can use the command [upsun project:convert](https://docs.upsun.com/administration/cli/reference.html#projectconvert)
> on this codebase to convert the existing `.platform.app.yaml` configuration file to the [Upsun Flex format](https://docs.upsun.com/create-apps/app-reference/single-runtime-image.html).

# Basic PHP for Platform.sh

This template provides the most basic configuration for running a custom PHP project built with Composer.  It includes but doesn't make use of the Platform.sh `config-reader` library.  It can be used to build a very rudimentary application but is intended primarily as a documentation reference.

PHP is a high-performance scripting language especially well suited to web development.

## Features

* PHP 8.0
* Automatic TLS certificates
* Composer-based build

## Customizations

The following files are of particular importance.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* The `.platform.app.yaml`, `.platform/services.yaml`, and `.platform/routes.yaml` files have been added.  These provide Platform.sh-specific configuration and are present in all projects on Platform.sh.  You may customize them as you see fit.
* A Composer library, [`platformsh/config-reader`](https://github.com/platformsh/config-reader-php), has been added.  It provides convenience wrappers for accessing the Platform.sh environment variables.

## References

* [PHP](https://php.net/)
* [PHP on Platform.sh](https://docs.platform.sh/languages/php.html)
