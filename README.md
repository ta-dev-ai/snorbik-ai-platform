# Snorbik AI Platform

**Plateforme IA locale pour développeurs** — utiliser des LLM en local dans Cursor, VS Code ou Codex, sans envoyer le code vers le cloud.

> Projet personnel · Python / FastAPI · Gateway OpenAI compatible · Ollama · Monitoring GPU

---

## Démo

![Démo Snorbik AI Platform — gateway locale, modèles et monitoring](assets/gifs/demo-2.gif)

**Ce que montre la vidéo :** une gateway IA locale branchée sur l'IDE, le catalogue de modèles et le suivi matériel (GPU) en temps réel.

---

## C'est quoi ?

Aujourd'hui, coder avec l'IA passe presque toujours par des API cloud (OpenAI, Anthropic…). Ça coûte cher, ça expose le code, et ça dépend d'une connexion externe.

**Snorbik AI Platform**, c'est ma réponse : une infrastructure IA **installée en local** qui se comporte comme une API OpenAI, pour que les outils de dev (Cursor, VS Code, Codex) puissent utiliser des modèles locaux (Ollama, HuggingFace) — **données et code restent sur la machine**.

---

## Ce que fait la plateforme

**MVP v1 — Gateway locale**
- API compatible OpenAI (`/v1/chat/completions`)
- Agents MCP pour connecter des outils externes
- Mode hybride local + cloud si besoin

**MVP v2 — Centre d'infrastructure IA**
- Catalogue et inspection des modèles installés
- Monitoring GPU / CPU / RAM en direct
- Interface web de supervision (FastAPI + frontend)

---

## Stack technique

| Domaine | Outils |
| ------- | ------ |
| Backend | Python, FastAPI |
| IA locale | Ollama, HuggingFace |
| Intégration IDE | OpenAI-compatible API, MCP |
| Monitoring | psutil, GPU telemetry |
| Frontend | JavaScript, thème VS Code |

---

## Liens

| | |
| --- | --- |
| **Démo web** | [ta-dev-ai.github.io/snorbik-ai-platform](https://ta-dev-ai.github.io/snorbik-ai-platform/) |
| **Repo** | [github.com/ta-dev-ai/snorbik-ai-platform](https://github.com/ta-dev-ai/snorbik-ai-platform) |

*Ce dépôt = démonstration publique du projet (GIF + description). Le code source applicatif complet reste privé.*
