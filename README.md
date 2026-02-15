# Servicelicense Module for FossBilling

Servicelicense is a FossBilling module designed for WordPress plugin vendors who need license key generation, secure ZIP distribution, and domain-bound validation.

This module allows automatic license creation per order and provides secure download access directly from the client area.

---

## Features

- Automatic license key generation
- Configurable license prefix and format
- Secure plugin ZIP download (session-based, no public file exposure)
- Per-product configuration
- Plugin version display in client area
- Changelog URL display
- Domain binding support
- Optional IP / hostname / path validation
- License reset from client panel
- Compatible with older orders (product config fallback)

## Requirements

- FossBilling 0.5.0+
- PHP 8.0+
- Writable `/data/downloads/` directory

## Installation

1. Download latest release ZIP
2. Extract into: /public_html/modules/Servicelicense
3. Clear FossBilling cache
4. Activate module inside admin panel

## Configuration

Inside Product → Module Settings:

- License prefix
- License length
- Plugin ZIP filename
- Plugin version
- Changelog URL
- Optional validation toggles

Upload your plugin ZIP into: /public_html/data/downloads

## How Download Works

The module uses a secure client controller route for downloads.  
Files are streamed via PHP and are never publicly exposed.

---

## License

MIT License

---

## Author

Bojan Denić   
https://www.kha.rs / https://www.kha-concepts.com


