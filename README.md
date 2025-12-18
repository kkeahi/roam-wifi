# Roam (*DubHacks 2025 Top Prize Winner*)

Roam is a mobile-controlled network gateway system. It allows businesses to monetize their internet connection using a Raspberry Pi gateway, while enabling users to easily find and purchase temporary WiFi access through a mobile app.

[DubHacks Devpost](https://devpost.com/software/roam-7h8vbm?_gl=1*gp1dzm*_gcl_au*MzUwOTM5MzY1LjE3NjA4NTE3Mjg.*_ga*MTM4OTI3NTU5LjE3NjA4NTE3Mjk.*_ga_0YHJK3Y10M*czE3NjYwMzc0NTQkbzMkZzEkdDE3NjYwMzc3ODIkajUxJGwwJGgw
)

> **Note:** This project was originally developed as a collaborative hackathon project.
> This repository represents my continued independent development and maintenance.

## Architecture

Roam is a two-part system:
1. **For Businesses:** A Raspberry Pi 5 acts as a secure network gateway. It routes traffic and enforces access control, ensuring only authorized devices can access the internet.
2. **For Users:** A React Native mobile application displays a Google Maps overview of participating businesses. Users can tap a location, pay a small fee via Stripe, and receive authorization to access the WiFi network for a preset timeslot.

## User Flow

1. **Business Setup:** The business connects the Raspberry Pi to their router via Ethernet to act as the gateway.
2. **Discovery:** The user opens the Roam app and selects an opted-in business (Raspberry Pi) node via the Google Maps API interface.
3. **Payment:** The user pays a small fee through the app for a specific duration of access.
4. **Access:** The user is connected to the network. If they need more time, they can extend their session directly through the app.
