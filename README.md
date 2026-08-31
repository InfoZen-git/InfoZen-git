<div align="center">

<img src="assets/header.svg" alt="InfoZen" width="100%">

<br>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=3200&pause=900&color=7AA2C8&center=true&vCenter=true&width=720&lines=Informatique+%C2%B7+R%C3%A9seaux+%C2%B7+Cybers%C3%A9curit%C3%A9;Hardware+%C2%B7+D%C3%A9veloppement+%C2%B7+Homelab;Open+Source+%C2%B7+Automatisation+%C2%B7+IA+locale;Construire.+Comprendre.+Am%C3%A9liorer." alt="InfoZen">

</div>

## À propos

**InfoZen** est un univers dédié à la technologie : développement, réseaux,
hardware, infrastructure, automatisation et expérimentation.

L'objectif : rendre la technologie **simple, utile et maîtrisable**, en construisant
des outils concrets, en documentant les expériences et en faisant évoluer des
infrastructures réelles.

| Domaine | Ce qu'InfoZen développe |
| :--- | :--- |
| **Développement** | Applications, outils open source, API et solutions sur mesure |
| **Infrastructure** | Réseaux, serveurs, Docker, self-hosting et supervision |
| **Hardware** | Montage PC, diagnostic, optimisation et électronique |
| **Automatisation** | Scripts, bots, services et workflows |
| **IA locale** | Expérimentation et intégration de modèles auto-hébergés |
| **Création tech** | Astuces, tutoriels et contenu autour de l'informatique |

---

## Projets

### Klyr-optimizer

**Optimiseur PC Windows open source.**

- 44 optimisations réparties en 6 modules
- Monitoring matériel intégré
- 5 outils avancés
- 100 % local, sans télémétrie
- Interface française et anglaise

**Technologies :** `C#` · `WPF` · `.NET` · `Windows`

[Voir le dépôt →](https://github.com/InfoZen-git/Klyr-optimizer)

---

### Homelab

Le homelab InfoZen sert de laboratoire pour expérimenter les réseaux,
l'auto-hébergement, Docker, l'automatisation, la supervision et l'IA locale.

```mermaid
flowchart LR
    NET([Internet]) --> LB[Livebox 7]
    REMOTE([Appareils distants]) -. Tailscale .-> RPI

    LB --> ZIMA["Serveur ZimaOS<br/>Docker"]
    LB --> RPI["Raspberry Pi 4B<br/>Docker"]

    ZIMA --> IA["IA locale<br/>Ollama + GPU"]
    ZIMA --> HA["Home Assistant"]
    ZIMA --> AGENT["Agent métriques<br/>FastAPI"]

    RPI --> API["API métriques<br/>FastAPI"]
    RPI --> HOLE["Pi-hole<br/>DNS filtrant"]
    RPI --> BOT["LeBonBot<br/>Discord"]
    RPI --> KUMA["Uptime Kuma<br/>Supervision"]

    AGENT -. HTTP .-> API
    ARD["Arduino Uno R4 WiFi<br/>Dashboard physique"] -. Wi-Fi / HTTP .-> API
```

**Infrastructure :** 2 hôtes Docker · 7 services auto-hébergés · réseau local · accès distant sécurisé.

---

### InfoZen-Link

**NFC & solutions numériques pour les professionnels.**

Le projet relie un support physique à une expérience numérique grâce au NFC
et aux QR codes, avec l'objectif de proposer des solutions simples et utiles.

```text
Support physique
       ↓
   NFC / QR Code
       ↓
Expérience numérique
       ↓
      Action
```

---

### LeBonBot

Projet d'automatisation autour de la recherche, du traitement et de la
publication d'annonces, avec une logique orientée vers la réduction des tâches répétitives.

---

## Ce que j'utilise

<div align="center">

<img src="https://skillicons.dev/icons?i=react,tailwind,js,python,fastapi,cs,dotnet&perline=7" alt="Technologies de développement">

<br><br>

<img src="https://skillicons.dev/icons?i=windows,linux,docker,raspberrypi,arduino,homeassistant&perline=6" alt="Technologies système et matériel">

<br><br>

<img src="https://skillicons.dev/icons?i=git,github,vscode,visualstudio&perline=4" alt="Outils de développement">

<br><br>

<sub>Ollama · Tailscale · Pi-hole · Uptime Kuma</sub>

</div>

---

## Architecture & infrastructure

```text
                         ┌─────────────────┐
                         │     INTERNET    │
                         └────────┬────────┘
                                  │
                         ┌────────▼────────┐
                         │    LIVEBOX 7    │
                         └────────┬────────┘
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
             ┌──────▼──────┐             ┌──────▼──────┐
             │   ZIMAOS    │             │ RASPBERRY PI│
             │    Docker   │             │    Docker   │
             └──────┬──────┘             └──────┬──────┘
                    │                           │
          ┌─────────┼─────────┐       ┌─────────┼─────────┐
          │         │         │       │         │         │
        IA       Home       API     DNS       Bot    Supervision
       locale  Assistant  métriques Pi-hole  Discord  Uptime Kuma

                         ╲       Tailscale       ╱
                          ╲──── accès distant ──╱
```

---

## Statistiques GitHub

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=InfoZen-git&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github" height="180" alt="Statistiques GitHub">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=InfoZen-git&layout=compact&theme=github_dark&hide_border=true&langs_count=8" height="180" alt="Langages les plus utilisés">

<br><br>

<img src="https://streak-stats.demolab.com?user=InfoZen-git&theme=github-dark-blue&hide_border=true" width="70%" alt="Série de contributions">

</div>

---

## Activité

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=InfoZen-git&theme=github-compact&hide_border=true&area=true&custom_title=Activité%20InfoZen%20sur%20GitHub" width="95%" alt="Activité GitHub">

</div>

---

## Philosophie

<div align="center">

### Construire.
### Comprendre.
### Expérimenter.
### Améliorer.

</div>

InfoZen ne se limite pas à utiliser des technologies : l'objectif est de les
comprendre, de les tester dans des conditions réelles et de transformer les
expérimentations en projets utiles.

---

## L'écosystème InfoZen

```text
                         ┌─────────────┐
                         │   INFOZEN   │
                         └──────┬──────┘
                                │
          ┌─────────────────────┼─────────────────────┐
          │                     │                     │
          ▼                     ▼                     ▼
    DÉVELOPPEMENT         INFRASTRUCTURE           HARDWARE
          │                     │                     │
          ▼                     ▼                     ▼
     LOGICIEL & API           HOMELAB             MONTAGE PC
          │                     │                     │
          ▼                     ▼                     ▼
    AUTOMATISATION          SELF-HOSTING          ÉLECTRONIQUE
          │                     │                     │
          └─────────────────────┼─────────────────────┘
                                │
                                ▼
                           INNOVATION
```

---

## Où retrouver InfoZen

<div align="center">

[![Portfolio](https://img.shields.io/badge/Portfolio-0b0c0e?style=flat-square&logo=googlechrome&logoColor=7aa2c8)](https://infozen-git.github.io/portfolio.github.io/)
[![YouTube](https://img.shields.io/badge/YouTube-0b0c0e?style=flat-square&logo=youtube&logoColor=7aa2c8)](https://www.youtube.com/@LesAstucesdInfoZen)
[![TikTok](https://img.shields.io/badge/TikTok-0b0c0e?style=flat-square&logo=tiktok&logoColor=7aa2c8)](https://www.tiktok.com/@infozen_off)
[![Instagram](https://img.shields.io/badge/Instagram-0b0c0e?style=flat-square&logo=instagram&logoColor=7aa2c8)](https://www.instagram.com/infozen_off)
[![Discord](https://img.shields.io/badge/Discord-0b0c0e?style=flat-square&logo=discord&logoColor=7aa2c8)](https://discord.gg/infozen)

<br>

<sub>Une idée, une question ou un projet ? InfoZen est là pour construire des solutions utiles.</sub>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3b82f6,50:172554,100:0b0c0e&height=100&section=footer" width="100%" alt="">

</div>
