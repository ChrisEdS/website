---
hide_title: true
sidebar_label: MailCrab
title: MailCrab | Self-Host on Easypanel
description: How to install MailCrab on Easypanel? 1-Click installation template for MailCrab on Easypanel
---

<!-- generated -->

# MailCrab

1-Click installation template for MailCrab on Easypanel

## Description

MailCrab is an email test server for development, written in Rust. It is inspired by MailHog and MailCatcher. The app allows users to view and inspect all incoming email, including formatted mail, attachments, headers, and raw mail contents. It runs on all amd64 and arm64 platforms using Docker. The backend server and frontend are both written in Rust. The backend receives email over an unencrypted connection on a configurable port and stores all email in memory while the application is running. The frontend communicates with the backend via an API and a websocket connection to receive and display email metadata and message contents. The app also supports commands to mark messages as opened or delete messages. MailCrab can be easily installed and run using Docker. TLS and authentication can be enabled for secure communication. The app can be configured with a prefix path and can be used behind a reverse proxy. By default, messages are stored in memory until the app is restarted, but a retention period can be set to automatically clear old messages. Sample messages are provided for testing purposes. The app can be developed and tested locally using Rust and Trunk.

## Benefits

- Easy email testing: MailCrab provides a simple and convenient way to test email functionality during development. It allows developers to easily view and inspect incoming email without the need for a real email server.
- Lightweight and efficient: MailCrab is written in Rust, which ensures high performance and efficient memory usage. The app stores email in memory while running, making it lightweight and fast.
- Flexible and customizable: MailCrab can be easily configured and customized to fit different development environments. It supports various options such as port configuration, TLS and authentication, prefix path, and integration with reverse proxies.

## Features

- Accept-all SMTP server: MailCrab acts as an SMTP server that accepts all incoming email. It can receive email over an unencrypted connection on a configurable port.
- Web interface: MailCrab provides a web interface to view and inspect all incoming email. Users can access the interface through a browser and perform actions such as viewing formatted mail, downloading attachments, viewing headers, and accessing the complete raw mail contents.
- API and websocket communication: MailCrab exposes an API that allows users to retrieve email metadata and message contents. The frontend communicates with the backend using the API and a websocket connection to receive real-time updates on new messages.
- Docker support: MailCrab can be easily installed and run using Docker. It provides a lightweight Docker image that can be deployed on all amd64 and arm64 platforms.
- TLS and authentication: MailCrab supports TLS and authentication for secure communication. It can generate a self-signed certificate or use a user-provided certificate for encryption. Any username/password combination is accepted.
- Path prefix: MailCrab can be configured with a prefix path for the web interface. This allows users to access the interface at a specific URL, such as http://localhost:1080/emails.
- Reverse proxy integration: MailCrab can be used behind a reverse proxy for additional security and flexibility. A reverse proxy guide is provided to assist with the integration.
- Retention period: By default, MailCrab stores messages in memory until the app is restarted. However, a retention period can be set to automatically clear old messages. This prevents memory overflow when the app receives a large number of messages.
- Development and testing: MailCrab can be developed and tested locally using Rust and Trunk. The backend server can be started using Cargo, and the frontend can be served using Trunk. Test messages are provided for testing purposes.

## Links

- [Github](https://github.com/tweedegolf/mailcrab)
- [Template Source](https://github.com/easypanel-io/templates/tree/main/templates/mailcrab)

## Options

Name | Description | Required | Default Value
-|-|-|-
App Service Name | - | yes | mailcrab
App Service Image | - | yes | marlonb/mailcrab:latest

## Screenshots

![MailCrab Screenshot](./assets/screenshot.png)

## Change Log

- 2022-11-5 – first release

## Contributors

- [Supernova3339](https://github.com/Supernova3339)
