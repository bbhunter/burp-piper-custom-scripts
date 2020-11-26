# Objective

Centralize and share all my custom scripts to be used with the [PIPER](https://portswigger.net/bappstore/e4e0f6c4f0274754917dcb5f4937bb9e) Burp extension.

[Documentation](https://blog.silentsignal.eu/2020/03/27/unix-style-approach-to-web-application-testing/) of the extension.

# Runtime requirements

> :information_source: No external dependencies.

Python >= **3.7** needed and in `PATH`.

```powershell
PS> python --version
Python 3.7.4
```

# Structure

Each script describes its goal in its header and for which PIPER tools is targeted to be used:

```text
"""
PIPER script to ...
Target tool: [PIPER_TOOL]
"""
```

# Overview of the scripts behavior

## detect-non-standart-headers

Add a comment to the matching line in the proxy tab.

![detect-non-standart-headers](images/detect-non-standart-headers.png)

## detect-request-to-web-api

Highlight the matching line in the proxy tab.

![detect-request-to-web-api](images/detect-request-to-web-api.png)

# Configuration

> :warning: Change the script location path defined in **prefix** field for all custom scripts **before** to import the configuration.

The file [piper-config.yaml](piper-config.yaml) contains the configuration that I use for all my custom scripts. 
