# RCity - CVE-2024-27198 (RCE & Admin Account Creation) & CVE-2024-27199 (Auth Bypass)
<b>Exploiting CVE-2024-27198 & CVE-2024-27199</b>

RCity is a Python script that interacts with a vulnerable TeamCity server. The CVE facilitates for unauthorised admin account creation, bypassing 403's on the domain. Whilst also achieving RCE, through the Debug/Processes route.

## Usage

To use the script, you need to provide the target TeamCity server URL as a command-line argument with the `-t` or `--target` argument: 

```bash
python3 RCity.py -t http://teamcity.com:8111
```

You can increase output verbosity with the `-v` or `--verbose` option:

```bash
python3 RCity.py -t http://teamcity.com:8111 --verbose
```

You can send one shot commands directly through `-c` or `--command` option, <b>if you want an interactive shell DO NOT use this option<b>:

```bash
python3 RCity.py -t http://teamcity.com:8111 -c id
```


## Features

- Admin Account Creation

- Remote Code Execution

- Generating Authorisation Tokens

- Enumerating Users

- Gathering Server Details

## Example

![image](https://github.com/Stuub/RCity/assets/60468836/0f604a31-aa75-491b-993a-1de4f3a707d6)

# RCE

![image](https://github.com/Stuub/RCity-CVE-2024-27198/assets/60468836/f6279e56-1b95-4295-9b04-8ccf825a03bd)

# Token Generation


![image](https://github.com/Stuub/RCity-CVE-2024-27198/assets/60468836/a6377923-ebdc-4119-bb70-f4dcbadac084)



## References

https://www.rapid7.com/blog/post/2024/03/04/etr-cve-2024-27198-and-cve-2024-27199-jetbrains-teamcity-multiple-authentication-bypass-vulnerabilities-fixed/

https://nvd.nist.gov/vuln/detail/CVE-2024-27198

https://github.com/W01fh4cker/CVE-2024-27198-RCE

## Disclaimer

This script is for educational purposes only. Use it responsibly and only on systems you have permission to access.
