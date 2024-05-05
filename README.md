# HyprOS
Arch Linux based operating system featuring Hyprland

> check **releases** section for prebuild ISO!

- **main** branch is development latest (unstable)

- **iso** branch is latest stable release

## Preview
coming soon..

## How to build ISO
Any Arch based system with installed **HyprOS** Repo is **required** to build the ISO.
- See [HyprOS](https://github.com/whatev33r/HyprOS-Repo) installation Guide.

**Step 1**: Install [Archiso](https://gitlab.archlinux.org/archlinux/archiso) utility:
```
pacman -Sy archiso
```
**Step 2**: Clone repository
```
git clone https://github.com/whatev33r/HyprOS-ISO.git
```
**Step 3**: Create work directory & build ISO
```
mkdir work
mkarchiso -v -w work HyprOS-ISO/ISO
```

### Base sources
- [Arch-ISO](https://gitlab.archlinux.org/archlinux/archiso)
- [ALCI](https://github.com/arch-linux-calamares-installer/alci-iso)
- [Hyprland](https://hyprland.org)

## Custom
> To access locally builded packages etc. on the ISO put files inside the [personal](ISO/airootfs/personal) directory.
 
> To adjust the available Cowspace (for live usage) change the **cow_spacesize** parameter in the [grub config](ISO/grub/grub.cfg).

## VM Notice
When using a VM, make sure you have 3D acceleration enabled in your virtio config (virt-manager) otherwise Hyprland **will not work**.
