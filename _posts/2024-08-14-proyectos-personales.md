---
layout: single
title: Proyectos Personales
excerpt: "Proyectos construidos de forma independiente para resolver problemas reales, explorar tecnologías y construir herramientas útiles en el ámbito industrial y personal."
date: 2026-04-05
classes: wide
header:
  teaser: 
  teaser_home_page: true
  icon: 
categories:
  - Proyectos Personales
tags:
  - Python
  - C#
  - Go
  - Docker
  - InfluxDB
  - Grafana
  - Telegraf
  - Telegram
  - WinCC
  - SCADA
  - HMI
  - Modbus
  - ESP32
  - Tailscale
  - Ollama
  - ChromaDB
  - Claude
  - SQLite
  - REST API
  - Linux
  - Git
  - GitHub
  - TIA Portal
  - TIA Openness
---

Proyectos desarrollados de forma independiente, orientados a resolver problemas reales del entorno industrial o a construir herramientas útiles para el trabajo diario. La mayoría han surgido de una necesidad concreta y varios han acabado desplegados en entornos de producción.

---

## Sistema de alarmas industriales por Telegram

**Stack:** Python · WinCC · ASEM HMI · Telegram Bot API

Sistema de notificación automática de alarmas industriales a grupos de usuarios mediante Telegram. Integrado con SCADA WinCC y HMI ASEM, con una arquitectura desacoplada que no impacta en el sistema SCADA existente. Desplegado en entornos reales de producción.

---

## Pipeline de documentación técnica con LLM

**Stack:** Python · C# · Claude API · REST API · SQLite · JSON

Pipeline de procesamiento batch de logs de campo mediante Claude API para generar documentación técnica estructurada. Incluye persistencia intermedia en JSON para auditoría y reprocesado, y publicación automática en wiki interna vía API REST. Implementación dual en Python y C# con base de datos compartida.

---

## Sistema de registros industriales

**Stack:** Grafana · InfluxDB · Telegraf · Docker

Sustitución de una solución de registro basada en hardware limitado por un stack moderno desplegado en Docker. Mejora drástica en tiempos de visualización de datos históricos y mayor flexibilidad para adaptarse a las necesidades reales de planta.

---

## Sistema de acceso remoto OT

**Stack:** Tailscale · Apache Guacamole · VNC · Docker

Arquitectura de acceso remoto seguro a sistemas industriales sin exposición directa a internet. Permite operar máquinas en planta de forma remota a través de un túnel cifrado, eliminando la necesidad de abrir puertos o depender de soluciones comerciales de terceros. Implementado en entornos productivos.

---

## MFA para HMI industrial

**Stack:** ESP32 · Modbus TCP · Go · TOTP

Sistema de autenticación de doble factor (TOTP) para HMIs industriales, sin dependencia de servicios cloud. Un ESP32 actúa como generador de códigos OTP accesible vía Modbus TCP desde la HMI. Incluye sincronización de hora entre HMI y dispositivo, y una variante implementada en Go para HMIs ejecutadas en PC.

---

## Sistema RAG para mantenimiento industrial

**Stack:** Python · ChromaDB · Ollama · Telegram Bot API

Sistema de consulta de conocimiento técnico construido sobre un histórico de averías. Utiliza embeddings locales con Ollama y ChromaDB para recuperar información relevante, con control de calidad mediante umbrales de similitud. Interfaz de consulta vía bot de Telegram.

---

## Time tracker con reporting automático

**Stack:** Python · SQLite · CSV · Ollama

Herramienta de registro de tiempo de trabajo con almacenamiento local en SQLite, exportación a CSV y generación automática de reportes mediante un modelo de lenguaje local con Ollama.

---

## Sistema de captura de conocimiento técnico *(en desarrollo)*

**Stack:** Python · SQLite

Herramienta interna para registrar problemas, soluciones y decisiones técnicas del trabajo diario de forma estructurada. Objetivo: evitar la pérdida de conocimiento y reducir la repetición de errores, construyendo una base de conocimiento compartida y consultable.

---

## Proyectos anteriores

**Sistema de alarmas WinCC (prototipo):** primera versión del sistema de alarmas por Telegram, desarrollada como prueba de concepto antes de su implementación profesional en Valfortec.

**TIA Openness:** herramientas en Python para interactuar con TIA Portal y optimizar flujos de trabajo — reducción de focos de error y mejora en tiempos de ejecución.

**Aplicaciones de escritorio:** proyectos en Rust con Tauri + React para herramientas con GUI distribuibles entre múltiples equipos. Aplicaciones en C# con Windows Forms.

**Homelab:** Raspberry Pi 4 con Debian Linux utilizada como host de bots de Telegram y servidor VPN. Punto de entrada al mundo Linux, SSH y Bash.
