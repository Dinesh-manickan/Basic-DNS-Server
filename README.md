# Basic DNS Server in Node.js

## Overview
This project is a simple DNS server implemented in Node.js, using the `dgram` module for handling UDP socket communication and the `dns-packet` module for encoding and decoding DNS packets. The server listens for DNS queries on port 53 and provides responses based on a predefined set of domain-to-IP mappings.

## Features
- **UDP Communication:** Uses the `dgram` module to handle UDP sockets for DNS queries and responses.
- **DNS Packet Handling:** The `dns-packet` module is utilized to decode incoming DNS requests and encode the appropriate responses.
- **Customizable Domain Mapping:** A predefined database allows for easy customization of domain-to-IP or CNAME mappings.
- **Authoritative Responses:** The server is designed to provide authoritative answers for the domains it manages.

## Project Structure
- **index.js**: The main server code that handles incoming DNS queries and sends out responses.
- **db.js**: The predefined database that contains the domain-to-IP and CNAME mappings.

## Getting Started

### Prerequisites
- Node.js installed on your machine.

### Installation
Install dependencies:
```bash
npm install
