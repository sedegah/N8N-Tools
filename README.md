# Uptime Monitor Workflow for n8n

This repository contains a reusable and customizable `n8n` workflow that periodically checks the availability of multiple web services and helps keep them awake (useful for free-tier hosting platforms like Render that sleeps due to inactivity).

## Features

- Periodically pings specified URLs every 10 minutes
- Supports multiple websites
- 10-second delay between each ping to avoid overload
- Configurable retry behavior per HTTP request
- Compatible with latest n8n versions (v1+)
- Simple to deploy and extend

## Setup Instructions

1. Clone or download this repository.
2. Open your n8n instance.
3. Go to the top-right menu → **Import workflow**.
4. Upload the `uptime-monitor.json` file.
5. Click **Activate** to start the monitoring.

## Use Case

This workflow is ideal for:
- Keeping Render/Vercel/Glitch/Free-hosted projects awake
- Monitoring service availability
- Lightweight uptime checking without external tools

## Notes

- You can easily modify the target URLs in each HTTP Request node.
- For extended functionality, consider adding:
  - Logging to a Google Sheet
  - Notifications via Email, Telegram, or WhatsApp
  - Downtime alerts with retries and delays

## License

This project is licensed under the MIT License.
