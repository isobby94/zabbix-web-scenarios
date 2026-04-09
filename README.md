# zabbix-web-scenarios
Zabbix template for monitoring web scenarios and HTTP endpoints

## Requirements
- Zabbix 7.0+

## Installation

### 1. Import template

Import template .yaml via Zabbix Web UI:
**Configuration → Templates → Import**

### 2. Add host

Add a new host (site name) in Zabbix and assign the **Web scenarios** template.

## Macros

| Macro | Default | Description |
|-------|---------|-------------|
| `{$PROTO}` | `https` | Protocol (http or https) |
| `{$PORT}` | | Port (e.g. :8080, leave empty for default) |
| `{$URL}` | | URL path (e.g. /health) |
| `{$RESPONSE_CODE}` | `200` | Expected HTTP response code |
