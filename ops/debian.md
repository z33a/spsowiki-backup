---
title: Debian
description: 
published: true
date: 2025-03-31T10:32:51.022Z
tags: 
editor: markdown
dateCreated: 2025-03-31T10:32:44.295Z
---

# Debian TUI - commands
## Nastavení NIC
- sudo nano /etc/network/interfaces

## Nastavení hostname
- 1. sudo nano /etc/hostname
- 2. sudo nano /etc/hosts (přepsat vedle domény)

## Založení uživatele
- sudo adduser ____

## Smazání + odstranění uživatele
- sudo deluser –remove-all-files ____

## Taskmanager
- sudo ss -tupan 

## SSH
- sudo apt install ssh

## Users
- w

## Setup
- pod root apt install sudo
- usermod -a -G sudo ____
- reboot

## Quota
- sudo nano /etc/fstab 
- pod #Home za defaults přidat -> ,usrquota
- reboot
- sudo apt install quota quotatool -y (quota a quotatool jsou diff packages)
- quotacheck -cu /home/
- quotaon /home/
- repquota /home/
- edquota _____ (user)