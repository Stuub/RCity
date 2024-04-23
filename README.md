# RCity - CVE-2024-27198 (RCE & Admin Account Creation)
<b>Exploiting CVE-2024-27198</b>

RCity is a Python script that interacts with a vulnerable TeamCity server. The CVE facilitates for unauthorised admin account creation, bypassing 403's on the domain. Whilst also achieving RCE, through the Debug/Processes route.

## Usage

To use the script, you need to provide the target TeamCity server URL as a command-line argument with the -t argument: 

```bash
python RCity.py -t http://teamcity.com:8111
```

You can increase output verbosity with the `-v` or `--verbose` option:

```bash
python RCity.py -t http://teamcity.com:8111 --verbose
```
## Features

Admin Account Creation

Remote Code Execution

Generating Authorisation Tokens

Enumerating Users

Gathering Server Details

## Example

![image](https://github.com/Stuub/RCity/assets/60468836/0f604a31-aa75-491b-993a-1de4f3a707d6)

## References

https://www.rapid7.com/blog/post/2024/03/04/etr-cve-2024-27198-and-cve-2024-27199-jetbrains-teamcity-multiple-authentication-bypass-vulnerabilities-fixed/

https://nvd.nist.gov/vuln/detail/CVE-2024-27198

https://github.com/W01fh4cker/CVE-2024-27198-RCE

## Disclaimer

This script is for educational purposes only. Use it responsibly and only on systems you have permission to access.
