# evf
evf stands for Errata verion finder and this simple tool is for finding all the Bugzillas for the given product, component, version and status of bugs. It scans all the comments in every bug and tries to find related errata. For every errata, it tries to find the corresponding release version of the product. This was originally implemented to find z-stream release versions of the OpenShift Container platform (for particular Bugzilla bugs).

## Configuration

Configuration is defined in the `config.yaml` file in the root of this repository. This file is required and you can find an example configuration file in the `example-config.yaml`. You have to provide your Bugzilla key (to be able to communicate with the Bugzilla API) and your Kerberos settings (to be able to comunicate with the errata API).

## How to run