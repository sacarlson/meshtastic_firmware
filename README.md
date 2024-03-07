# Meshtastic Firmware

![GitHub release downloads](https://img.shields.io/github/downloads/meshtastic/firmware/total)
[![CI](https://img.shields.io/github/actions/workflow/status/meshtastic/firmware/main_matrix.yml?branch=master&label=actions&logo=github&color=yellow)](https://github.com/meshtastic/firmware/actions/workflows/ci.yml)
[![CLA assistant](https://cla-assistant.io/readme/badge/meshtastic/firmware)](https://cla-assistant.io/meshtastic/firmware)
[![Fiscal Contributors](https://opencollective.com/meshtastic/tiers/badge.svg?label=Fiscal%20Contributors&color=deeppink)](https://opencollective.com/meshtastic/)
[![Vercel](https://img.shields.io/static/v1?label=Powered%20by&message=Vercel&style=flat&logo=vercel&color=000000)](https://vercel.com?utm_source=meshtastic&utm_campaign=oss)

## Overview

This repository contains the device firmware for the Meshtastic project.  This branch is only for a few problems I personaly found for the now discontinued support heltec lora32 v2.1 that had some power supply issues and a minor bug fix to prevent lockup when setting RF power levels bellow 2db.  If this was to be pushed to meshtastic it would have to be tested and most likely modified to continue to work with other newer devices now supported by meshtastic.  With this version I am able to run the old heltec v2.1 on a small 5w solar panel and a 1000mah lipo battery without problems.  If I want long duration 10+ day operation with no solar power on just 1000ma battery I can set power>adc multiplier overide to 2.7v and set super deep sleep duration to 20000 sec.  This will make the voltage telemetry numbers seen incorect but still works if needed.

- **[Building Instructions](https://meshtastic.org/docs/development/firmware/build)**
- **[Flashing Instructions](https://meshtastic.org/docs/getting-started/flashing-firmware/)**

## Stats

![Alt](https://repobeats.axiom.co/api/embed/a92f097d9197ae853e780ec53d7d126e545629ab.svg "Repobeats analytics image")
