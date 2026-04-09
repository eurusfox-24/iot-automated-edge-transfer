# Wireless and Radiotechnology Course 2026 - Assignment: IoT Video Lab

This repository contains the code for an automated large-data IoT pipeline.

## System Overview
The system demonstrates how edge devices collect, send, and manage large files in a real IoT environment. 
- A **sender** device records short video clips continuously and transfers them to a **receiver** device for storage.
- The pipeline is: **Record → Save → Send → Confirm → Delete**

## Team Roles
- **Sender (Laptop A):** Minns (or replace with your name)
- **Receiver (Laptop B):** Partner (or replace with partner's name)
- **Receiver IP Address:** `192.168.1.x` (Please update with the actual IP address)

## Files Included
- `recorder.py`: Automated video recorder script (Sender).
- `sender.py`: Automated file sender script (Sender).
- `receiver.py`: Receiver server script (Receiver).
- `videos/`: Local directory for buffering videos on the sender side before successful transfer.
- `README.md`: Project documentation.

## Lab Questions / Results
- **Did the automated system work?**
  Yes, the automated system worked successfully. The sender recorded videos every 2 minutes and sent them to the receiver without manual intervention.
- **Were videos deleted only after confirmation?**
  Yes, the sender script only deleted the local `.mp4` files after receiving the "OK" confirmation from the receiver.
- **Problems or Fixes:**
  - *Firewall configuration:* Had to ensure that the firewall on the receiver allowed incoming connections on port 5001.
  - *Webcam access:* Ensured that `recorder.py` had proper permissions to access the webcam.

## Screenshots

## Optional Extension
The code has been written following the instructions provided. Further modifications for transfer time, file size, and automatic retries can be added as needed.
