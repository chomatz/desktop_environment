# desktop_environment
ansible role for gnome deployment

## requirements

## variables
- grub_menu_resolution: 1920x1080
  - set to the desired resolution

## dependencies
requires the following role(s):
- [boot_loader](https://github.com/chomatz/boot_loader)

## examples
```
- name: deploy gnome desktop
  ansible.builtin.include_role:
    name: desktop_environment
    tasks_from: gnome_desktop.yml
```
```
- name: deploy gnome tweaks
  ansible.builtin.include_role:
    name: desktop_environment
    tasks_from: gnome_tweaks.yml
```
