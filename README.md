# playbook

Ansible playbooks.

## Usage

```powershell
$ ansible-playbook main.yaml --tags <tag>
```

To list the available tags:

```powershell
$ Install-Module -Name powershell-yaml
$ Import-Module powershell-yaml
$ gc -Raw main.yaml | ConvertFrom-Yaml | % { $_.tags } | sort -Unique | Join-String -Separator ', '
```
