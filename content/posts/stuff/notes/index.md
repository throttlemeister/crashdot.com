+++
title = 'Quick reference notes'
date = 2024-11-30T22:58:17+01:00
draft = true
tags = ["opensuse", "linux", "notes"]
+++
## Introduction

This is a page where I store quick notes and commands I sometimes need but always forget and end up having to search for on the web, which is not the most economic way to spend my time. They are generally not very complicated, but not used quite enough to always memorize. Me lazy..

This is a living document. Things will be added as I go.

## Update-alternatives

Installing neovim on OpenSUSE does not make it recognized automatically as an alternative for vi. We will need to add it manually for it to be used and set by default.

## pbl - configure or install bootloader

pbl is a commandline utility that allows you to configure the bootloader, add options, etc and saves that configuration in `/etc/kernel/cmdline`

    Usage: pbl [OPTIONS]
    Configure/install boot loader.

    Options:
        --install                   Install boot loader.
        --config                    Create boot loader config.
        --show                      Print current boot loader.
        --loader BOOTLOADER         Set current boot loader to BOOTLOADER.
                                    Supported values: none, grub2, grub2-bls, grub2-efi, systemd-boot, u-boot.
        --default ENTRY             Set default boot entry to ENTRY.
        --add-option OPTION         Add OPTION to default boot options (grub2).
        --del-option OPTION         Delete OPTION from default boot options (grub2).
        --get-option OPTION         Get OPTION from default boot options (grub2).
        --add-kernel VERSION [KERNEL [INITRD]]
                                    Add kernel with version VERSION. Optionally pass kernel and initrd
                                    explicitly (systemd-boot).
        --remove-kernel VERSION     Remove kernel with version VERSION (systemd-boot).
        --default-settings          Return default kernel, initrd, and boot options.
        --log LOGFILE               Log messages to LOGFILE (default: /var/log/pbl.log)
        --version                   Show pbl version.
        --help                      Write this help text.

## Quick reference on some vi commands

Select block:  ^V to enter block mode, use arrow to position cursoruse
Edit: use SHIFT-i to switch to insert, ESC to apply

Realign all idents: gg=G