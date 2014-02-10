# Ash's Development Kit

This is an [Ansible](http://docs.ansible.com/index.html) playbook that provisions a server with
a non-root account, sudo rights, configured [dotfiles](https://github.com/smashwilson/dotfiles), and a
bunch of other tools that I pretty much always want to be present.

## Usage

Modify `user` and `github_user` within `vars.yml` to match you, then run:

```bash
echo "host-ip" >> hosts
ansible-playbook -i hosts site.yml
```
