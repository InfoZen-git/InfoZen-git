<img src="assets/header.svg" alt="InfoZen, par Octave" width="100%">

## À propos

Sous le nom **InfoZen**, je partage des astuces tech au quotidien,
je développe des outils open source, je fais tourner mon propre homelab et j'en tire des
activités bien réelles.

L'idée derrière tout ça : rendre la technologie simple, utile et un peu plus zen.

|  |  |
| :--- | :--- |
| **Créateur** | Formats courts sur TikTok et Instagram, tutos sur YouTube |
| **Développeur** | Outils open source et applications sur mesure |
| **Homelab** | Deux hôtes Docker, sept services auto-hébergés |
| **Entrepreneur** | Prestation, développement client, revente, produits locaux |

## Projets

### Klyr-optimizer

Optimiseur PC Windows open source, écrit en C# et WPF.

* 44 optimisations réparties en 6 modules
* Monitoring matériel intégré, plus 5 outils avancés
* 100 % local, aucune télémétrie
* Interface disponible en français et en anglais

**[Voir le dépôt](https://github.com/InfoZen-git/Klyr-optimizer)**

### Homelab

Mon terrain de jeu réseau à la maison, et la source de la moitié de mes idées.
Une Livebox 7 en tête de pont, un switch stacké pour la distribution, un TP-Link
Archer AX3000 en Wi-Fi 6, puis deux hôtes Docker qui font tourner l'ensemble.

```mermaid
flowchart LR
    NET([Internet]) --> LB[Livebox 7]
    REMOTE([Appareils distants]) -. Tailscale .-> RPI

    LB --> ZIMA["Serveur ZimaOS<br/>Docker"]
    LB --> RPI["Raspberry Pi 4B<br/>Docker"]

    ZIMA --> IA["Négociateur IA<br/>Ollama, GPU"]
    ZIMA --> HA["Home Assistant"]
    ZIMA --> AGENT["Agent métriques<br/>FastAPI"]

    RPI --> API["API métriques<br/>FastAPI"]
    RPI --> HOLE["Pi-hole<br/>DNS filtrant"]
    RPI --> BOT["LeBonBot<br/>Discord"]
    RPI --> KUMA["Uptime Kuma<br/>supervision"]

    AGENT -. HTTP .-> API
    ARD["Arduino Uno R4 WiFi<br/>dashboard physique"] -. Wi-Fi, HTTP .-> API
```

## Ce que j'utilise

![React](https://img.shields.io/badge/React-0b0c0e?style=flat-square&logo=react&logoColor=7aa2c8)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-0b0c0e?style=flat-square&logo=tailwindcss&logoColor=7aa2c8)
![JavaScript](https://img.shields.io/badge/JavaScript-0b0c0e?style=flat-square&logo=javascript&logoColor=7aa2c8)
![Python](https://img.shields.io/badge/Python-0b0c0e?style=flat-square&logo=python&logoColor=7aa2c8)
![FastAPI](https://img.shields.io/badge/FastAPI-0b0c0e?style=flat-square&logo=fastapi&logoColor=7aa2c8)
![.NET](https://img.shields.io/badge/.NET-0b0c0e?style=flat-square&logo=dotnet&logoColor=7aa2c8)

![Docker](https://img.shields.io/badge/Docker-0b0c0e?style=flat-square&logo=docker&logoColor=7aa2c8)
![Linux](https://img.shields.io/badge/Linux-0b0c0e?style=flat-square&logo=linux&logoColor=7aa2c8)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-0b0c0e?style=flat-square&logo=raspberrypi&logoColor=7aa2c8)
![Home Assistant](https://img.shields.io/badge/Home_Assistant-0b0c0e?style=flat-square&logo=homeassistant&logoColor=7aa2c8)
![Ollama](https://img.shields.io/badge/Ollama-0b0c0e?style=flat-square&logo=ollama&logoColor=7aa2c8)
![Tailscale](https://img.shields.io/badge/Tailscale-0b0c0e?style=flat-square&logo=tailscale&logoColor=7aa2c8)
![Pi-hole](https://img.shields.io/badge/Pi--hole-0b0c0e?style=flat-square&logo=pihole&logoColor=7aa2c8)
![Arduino](https://img.shields.io/badge/Arduino-0b0c0e?style=flat-square&logo=arduino&logoColor=7aa2c8)

## Où me trouver

[![Portfolio](https://img.shields.io/badge/Portfolio-0b0c0e?style=flat-square&logo=googlechrome&logoColor=7aa2c8)](https://infozen-git.github.io/portfolio.github.io/)
[![YouTube](https://img.shields.io/badge/Les_Astuces_d'InfoZen-0b0c0e?style=flat-square&logo=youtube&logoColor=7aa2c8)](https://www.youtube.com/@LesAstucesdInfoZen)
[![TikTok](https://img.shields.io/badge/@infozen__off-0b0c0e?style=flat-square&logo=tiktok&logoColor=7aa2c8)](https://www.tiktok.com/@infozen_off)
[![Instagram](https://img.shields.io/badge/@infozen__off-0b0c0e?style=flat-square&logo=instagram&logoColor=7aa2c8)](https://www.instagram.com/infozen_off)
[![Discord](https://img.shields.io/badge/Discord-0b0c0e?style=flat-square&logo=discord&logoColor=7aa2c8)](https://discord.gg/infozen)
[![Mail](https://img.shields.io/badge/contact.infozen68@gmail.com-0b0c0e?style=flat-square&logo=gmail&logoColor=7aa2c8)](mailto:contact.infozen68@gmail.com)

<br>

<sub>Une idée, une question, un projet ? Le Discord est ouvert, et beaucoup de choses y démarrent d'un simple message.</sub>
