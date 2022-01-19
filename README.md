# Archlinux server hardening Ansible rules

This is a set of Ansible rules to harden an Archlinux server.

Hardening rules are based on the following Guide CIS: `CIS_Distribution_Independent_Linux_Benchmark_v2.0.0.pdf`

## Usage

The host file defines the hosts to apply rules. Change `srv` with the ip of your server.

Make sure to review the variables in the file `harden.yaml`.

To apply the rules run the following command.

```bash
>_ ansible-playbook harden.yaml -K -e "user=<username>" -k -i hosts
```

## TODO

At this time only ssh is hardened!
