---
sidebar_position: 1
---

# Tutorial Introduction

This is a quick-start guide for using Meshtastic in and around Memphis. This is meant to augment the official documentation and other sources.

## Getting Started

[Follow the getting started guide first](https://meshtastic.org/docs/getting-started/).

## Configure Your Node

### LoRa Config

| Setting | Value |
|---------|-------|
| Region | United States |
| Ok to MQTT | True (optional -- results in your data being published online) |

### Channels - 0 Default

| Setting | Value |
|--------|--------|
| Positions Enabled | True|

### User

| Setting | Value |
|---------|-------|
| Long Name | A descriptive name identifying you and this particular node |
| Short Name | A short, unique abbreviation for your node |
| Licensed Operator | False (required to be able to connect properly) |

### Position

| Setting | Value |
|---------|-------|
| Smart Position Minimum Interval | Two Minutes |
| Device GPS | Disabled and Fixed Position for fixed nodes |

## Additional Configuration to Uplink

If you'd like your node to contribute to the mesh via the internet and serve as an uplink, follow these additional steps:

### Module Configuration: MQTT

| Setting | Value |
|---------|-------|
| Enabled | True |
| Map Report Enabled | True |
| Root Topic | msh/US/memphismesh.com |

### Channels: 0 Primary

| Setting | Value |
|--------|--------|
| MQTT Uplink Enabled | True |
