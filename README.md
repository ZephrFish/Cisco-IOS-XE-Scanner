# Cisco-IOS-EX-Scanner (CVE-2023-20198)
CVE-2023-20198 &amp; 0Day Implant Scanner (tested in a lab and works, YMMV)

Quick and dirty scanner to run checks if the host is vulnerable/been compromised using 0day in Cisco IOS XE. This tool is designed to scan a given target or a list of targets to determine potential vulnerabilities based on specific checks.

## Reqs
```
pip install requests
```
## Usage
You can use the XE Implant Scanner in two modes: Single target mode and multiple targets mode (using an input file).

### Single Target Mode:

```
python XEImplantScanner.py --rhost [TARGET_IP_OR_DOMAIN] [--rport PORT_NUMBER] [--ssl]
```
#### Arguments:

- --rhost : The IP address or domain name of the target.
- --rport : The port number to scan (default is 80).
- --ssl : Use this flag to enable SSL.

### Multiple Targets Mode (Using an Input File):

```
python XEImplantScanner.py --input_file [FILE_NAME] [--rport PORT_NUMBER] [--ssl]
```

#### Arguments:

- --input_file : A file containing a list of IP addresses or domain names to scan, one per line.
- --rport : The port number to scan (default is 80).
- --ssl : Use this flag to enable SSL.
