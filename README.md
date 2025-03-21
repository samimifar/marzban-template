# marzban-template

A modern, lightweight, and powerful subscription page template for [Marzban](https://github.com/Gozargah/Marzban) written in HTML and CSS.

<p align="center">
  <a href="https://github.com/samimifar/marzban-templates" target="_blank" rel="noopener noreferrer" >
    <img src="https://github.com/samimifar/marzban-template/blob/main/img/marzban-template.png" alt="SubPage screenshots" width="800" height="auto">
  </a>
</p>

## Introduction

A simple yet effective subscription template (written in plain `HTML` and `CSS`) to enhance the user experience of Marzban's subscription page.

## Features

- Quickly add subscriptions to **v2rayNG, Streisand**.
- Direct download links for required applications.
- Clean and minimal design optimized for performance.
- Supports `English`, `Farsi/Persian` and `Russian` languages.

## Installation

1. Download the template file
   <br><br>
   **English:**
   ```sh
   sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/samimifar/marzban-template/master/src/en/index.html
   ```
   
   **Russian:**
   ```sh
   sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/samimifar/marzban-template/master/src/en/index.html
   ```
   
   **Persian/فارسی:**
   ```sh
   sudo wget -N -P /var/lib/marzban/templates/subscription/ https://raw.githubusercontent.com/samimifar/marzban-template/master/src/fa/index.html
   ```
   
3. Configure Marzban to use the custom template by running
   ```sh
   echo 'CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"' | sudo tee -a /opt/marzban/.env
   echo 'SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"' | sudo tee -a /opt/marzban/.env
   ```
   Alternatively, manually add the following lines to your `.env` file located at `/opt/marzban`:
   ```sh
   CUSTOM_TEMPLATES_DIRECTORY="/var/lib/marzban/templates/"
   SUBSCRIPTION_PAGE_TEMPLATE="subscription/index.html"
   ```
4. Restart Marzban
   ```sh
   marzban restart
   ```

## Add support Link and Button

to add your support link as button edit the file and add your support link in line `5`
 ```js
   const SupportID = "PUT YOUR LINK HERE"; // Fill with your support link or keep it blank to hide Support section 
   ```

## Update

To update the template, simply repeat **Step 1** of the installation process.

## License

**All intellectual and material rights of this project belong to:**  

Samimifar [![Telegram](https://img.shields.io/badge/Telegram-26A5E4?logo=telegram&logoColor=white)](https://t.me/samimifar)

---

## Support Me

If you like this project and want to support its development, you can donate using crypto:

- **TON:** `UQAtCP3gnHhb5QRy-3fnAqwXBg_AV4vT1jH5MtaCYNTOv7v4`
- **TRX:** `TDKJrRtZirFf95RZ9VUo5ERkmz3x8MXbUN`
- **USDT (BEP20):** `0x49bA8498e5d619f1bA208fB57B8b860C98700652`
