# server-home-deployment-ansible
Overview:

1. Host your Ansible playbooks in a Git repository (private if preferred).
2. Run an Ansible control node in a lightweight VM or LXC container on your Proxmox server.
3. Use Ubuntu's Autoinstall (or Debian's Preseed if you prefer Debian) for unattended Linux installations.
4. Have the installer add your SSH key and install a small bootstrap script.
5. After first boot, use ansible-pull so laptops configure themselves from this Git repo.
6. Organize playbooks into reusable roles (base system, development, media, gaming, etc.) to mix and match configurations for different laptops.
