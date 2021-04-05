# tools

The aim of this project is to provide some frequently used tools and mini-scripts onto your local Ubuntu workstation. These tools provide some additional commands that can be used to perform routine tasks.

## Getting Started

The following instructions will help you to get a copy of the project installed onto your local machine.

After the initial checkout of the project, you will first need to "install the installer" in order that you can install the tools that you need from those that are available within the project.

From your checked out repo, run the following command with elevated permissions (sudo), as necessary for your local environment:

```
./add-tools add-tools
```

## Installing tools ##

Once `add-tools` is working on your workstation, simply add any new tool you need by executing, followed by the name of the tool you wish to enable.

Example:
```
add-tools dns
```
The above will add the `dns` tool to your local filesystem


## Tools syntax ##

Typically, each tool can be run from anywhere on your filesystem by calling it, followed by the expected parameters. A `version` and `help` flag have been added, and can be called to find the version of the tool plus any basic syntax specific to it.

Example:
```
dns help
```
returns the expected syntax required to run this script, e.g. `dns FQDN`, which in turn will display as follows, where FQDN is substituted for a valid and fully qualified domain name :
```
$ dns github.com
Checking DNS records for github.com
github.com.		18	IN	A	140.82.118.3
<End>
```

## Available Tools ##

At the present time, the available tools contained inside this repository are as follows:

| Command | Description |
| --- | --- |
| `add-tools` | Installs a tool onto your local filesystem |
| `cert` | Extracts and displays data from a variety of different SSL cert files, e.g. `pfx` |
| `cxn` | Provides a connection to a mapped server or environment. |
| `dns` | Returns some useful DNS information from `dig` using a given fully qualified domain name |
| `extract` | Extracts and outputs to file, details from a valid Apache or IIS configuration. |
| `get` | Performs a wget using a provided username and password to test 401-auth |
| `jb` | Provides tools for managing the DQM platform, and running reports. |
| `killm` | is a simple `kill -9` command run against a parameter submitted by the user. |
| `mcurl` | Executes a loop of curl commands on a specific URL and returns the length |
| `pid` | Displays any locally running process containing a given string |
| `test-redirect` | Tests a URL through a dedicated redirect service |


## Updating and maintaining tools ##

To update tools, simply perform a `git pull` on your checked-out *develop* branch
To ensure that your tools continue to work, do not delete the repository, or any files within it.


## Development and contribution ##

Although this is largely a private toolset, created for personal use, enhancements and additions are welcome. Please create your feature branch from `develop` and submit a pull request in the usual way. Alternatively, create a separate fork or local repository based on an initial clone of the main repository, and use your own version.

The above tools are considered to be in development at all times, as there are often additional modifications and other features added to the existing toolset.

The author will not provide any access keys.

## Disclaimer ##

Whilst none of the above tools write data, usage of the tools in this repository is free of charge, but the sole responsibility of any person who decides to install and execute any of the contained syntax, and therefore accepts any risk involved.

I hope there is something useful for you.
