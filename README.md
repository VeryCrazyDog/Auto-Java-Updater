# Auto-Java-Updater
Keep Java up to date in Windows! Remove redundant installations!

Java has one MAJOR flaw in windows. You can't keep it up to date automatically. The "Auto Update" feature just downloads new updates, and doesn't install them unless you click. Also when it does install a new version, it doesn't remove the old version. That wastes space and is no good. The software helps. Schedule it to run every day and it will keep your JRE running happy!

This updater only update 32-bit version of JRE.

Windows XP is not supported. Tested in Windows 7 64 bit.


## Installation
You will need to cURL in order to run the script. You may:

1. Configure it manually by download it from https://curl.haxx.se/download.html.
2. Allow this script to install it automatically by setting options `dontInstallCurl` to `0` and `verifySSL` to `0`. Please notice that the installation file used in automatic installation is provided by the original author of this script **Grintor** and does not support certificate verification. Use at your own risk.


## Usage
Double click `javaUpdate.cmd` to run the updater. Alternatively you can configure to run the updater in scheduled task.


## Configurable Options
There are some configurable options available. Open `javaUpdate.cmd` and edit them in the top of the file.

- `dontInstallCurl`: Whether to automatically install required program cURL. Set it to `0` to allow automaitc installation. Default is `1`.
- `verifySSL`: Whether to verify the certificate when connect to server via HTTPS. Set it to `0` to disable verification. Default is `1`.
- `installJavaIfMissing`: Whether to install JRE if none is found. Set it to `1` to install JRE when none is found. Default is `0`.


## Credit
Thanks **Grintor** for the [initial work on this script](https://github.com/grintor/Auto-Java-Updater). Thanks users who [reported issues](https://github.com/grintor/Auto-Java-Updater/issues) and issued [pull request](https://github.com/grintor/Auto-Java-Updater/pull/3) to the original script so that I am able to make more adjustment and enhancement.


## License
This program is free software.

This program IS PROVIDED WITHOUT WARRANTY, EITHER EXPRESSED OR IMPLIED.

This program is copyrighted under the terms of GPLv3, see https://www.gnu.org/licenses/gpl-3.0-standalone.html
