---
title: A fun hardware project - tracking BLE devices that pass by my window
---

# Intro

This semester my girlfriend is taking a class called wearable technology, she needed my help to build and code an arduino that would change colors on her earings based on what site she was on and whether someone could disturb her or not.

Helping her with that sparked something in me and made me want to tinker some more.

# The idea

The first thing that came to my mind is data. I love it, and love doing things with it. Since her project used bluetooth to communicate, thats where I started to.

The idea is to have an arduino that logs all the bluetooth devices it detects and the timestamp when it was detected, then send that data over wifi to a server that adds it to a database.

Then once I have the data, I can find out which devices are seen around that same times (and clean out the devices that are in my building). 

I am curious what I will find!

# Hardware

To start I am just planning on using an Arduino R4 (usb-c, wifi, BLE), and my mini-pc from my old homelab project to host the server with the database.

![The arduino R4](/assets/homelab/r4.jpeg)
![My Mini-pc](/assets/homelab/mini-pc.jpeg)


# Getting started

Honestly I didn't know much about Bluetooth, and I have been learning more. But I was particularly disapointed to learn that the bluetooth on the arduinio (BLE) may not be able to detect the phones and other normal bluetooth devices that pass by (not even 100% sure of this now still trying to learn).


I already got the arduino to connect to my wifi and detect BLE devices, next I want to setup the postgres database I will be using and start collecting data!


