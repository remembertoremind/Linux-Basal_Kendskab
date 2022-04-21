---
aspectratio: 43
author: Christian
title: Kursus i Linux
subtitle: Part 5 - System og bash
date: \today
institute: Rådet for større IT-sikkerhed
header-includes:
- \titlegraphic{ \includegraphics[width=1.7cm]{../images/linux.jpg}}
slide_level: 2
theme: "Dresden"
toc: false
---

# Introduktion

## Hvad vi skal gennem
- Noget om hosts
- Noget om brugere
- Noget om filer
- Noget om logs
- Noget om bash

# Noget om hosts

## Hardware
- lsmem
- lscpu
- lspci
- lsusb

## Drivere
- lsmod
- lsmod | grep \$MOD
- lsmod | less

## Netværk
- ip -a
- nmtui
- ping \$IP
- check port
	- telnet \$IP \$PORT
	- nc/netcat \$IP \$PORT

# Brugere

## Brugere
- who
- lslogins

# Filer

## Filer
- Se hvilke filer der er åbne lige nu
	- lsof
- Se hvilke processer der kører
	- ps

## Andet relevant
- timedatectl
- hostnamectl
- uname -a

# Logs

## Logfiler
- Check /var/log
- journalctl -f
- sudo dmesg -w

## Programmer
- which \$PROGRAM
- whereis \$PROGRAM

## Manualer
- apropos \$PROGRAM
- man \$PROGRAM

# Bash

## Bourne again shell: key-binds
| **key-bind** | **resultat**                  |
| :---         | ---                           |
| ctrl+r       | Gå tilbage i history          |
| ctrl+l       | Clear screen                  |
| ctrl+a       | Gå til start                  |
| ctrl+e       | Gå til slut                   |
| ctrl+w       | Slet forrige ord              |
| ctrl+u       | Slet før cursor               |
| ctrl+k       | Slet efter cursor             |
| ctrl+y       | Print slettet tekst           |
| ctrl+x+e     | Edit kommando inden afvikling |

## Bourne again shell: Commands

| **cmd** | **resultat**                        |
| :---    | ---                                 |
| pwd     | print dir                           |
| cd -    | gå til forrige dir                  |
| cd ..   | Gå op                               |
| cd      | Gå til home                         |
| cd ~/   | Gå til home                         |
| sudo !! | Forrige kommando + sudo             |

## Bourne again shell: alias
Man kan lave nogle ret fede ting med alias ved at rette i sin ~/.bashrc

    alias p='something something'

Check hvilke alias der allerede er

    alias

## Bourne again shell: environments
- printenv
- tilføj eller fjern i ~/.bashrc

    export EDITOR=vim
    export BROWSER=qutebrowser

# Afslutning

## Spørgsmål

![Spørg](../images/spoerg.jpg){ width=70% }

## Sidste slide

5 min pause
