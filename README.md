&nbsp;

# <span style="color: rgb(53, 152, 219);">Ansible Ad-hoc Commands</span>

## <span style="color: rgb(241, 196, 15);">Syntax</span>

```bash
ansible host-pattern -m module [-a 'module arguments'] [-i inventory]

```

<span style="color: rgb(230, 126, 35);">**Example:**</span>

```bash
ansible all -m ping
# For sudo, use logname command to get the original username
ansible all -m ping -u $(logname)

```

To list the matching managed hosts without executing anything:

```bash
ansible --list-hosts

