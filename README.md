# Flask + Redis — Docker Compose Project

A hands-on Docker Compose project built to understand how multiple containers work together.

The application consists of a Flask web application and a Redis backend, deployed on an AWS EC2 Ubuntu server.

## Architecture

```text
                    AWS EC2
                       |
                       v
                  Docker Compose
                       |
              +--------+--------+
              |                 |
              v                 v
        Flask Container    Redis Container
              |                 |
              +--------+--------+
                       |
                Docker Network
                       |
                       v
                Redis Named Volume
