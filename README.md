# apn-web_1.0.3_all.ipk
<img src="https://www.ilblogdicristiangallo.com/wp-content/uploads/2025/10/1000146365.jpg" alt="Immagine dal blog di Cristian Gallo"></img>

The apn-web.ipk package enables automatic APN configuration for all Italian mobile operators directly from a web interface, accessible via both desktop and mobile browsers.

# Description

apn-web_1.0.3_all.ipk is an OpenWrt package that provides automatic APN configuration for all Italian mobile operators through a web interface. The interface works on both desktop and mobile browsers and is designed to configure WAN connections using either the QMI protocol, ModemManager and MBIM Cellular, which can now be selected directly from the apn.html page.

If the WAN interface is already configured as qmi, modemmanager (cellular) and mbim Cellular, the system automatically detects the active APN and pre-fills it in the interface, making the setup even easier. Just click Apply Configuration to activate the changes.

Features

Predefined APN selector (TIM, Vodafone, WindTre, Iliad, etc.)

IP type selection: IPv4, IPv6, IPv4v6

Optional SIM PIN input

Automatic APN pre-fill if WAN is active (QMI, ModemManager and MBIM Cellular)

Modem type selection: QMI, ModemManager and MBIM Cellular

Buttons for:

Applying configuration

Restarting WAN

Rebooting the router

Copying selected APN

Localized success/error messages (Italian/English)

Responsive layout for smartphones and tablets

# Requirements

OpenWrt router with 4G-5G modem

QMI-compatible modem (cdc-wdm), ModemManager-compatible modem and MBIM Cellular-compatible modem

WAN interface configured as qmi, modemmanager and MBIM Cellular

# Installation
# Method 1: WinSCP (Windows)

Connect to your router using WinSCP:

Protocol: SCP

Host: 192.168.1.1

Port: 22

Username: root

Password: (blank or your router password)

Upload the file apn-web_1.0.3_all.ipk to the /tmp directory

Open a terminal (via PuTTY or WinSCP) and run:

<pre>opkg install /tmp/apn-web_1.0.3_all.ipk</pre>

# Method 2: SCP (Linux/macOS)

Copy the file to your router:

<pre>scp apn-web_1.0.3_all.ipk root@192.168.1.1:/tmp/</pre>


SSH into the router:

<pre>ssh root@192.168.1.1</pre>


Install the package:

<pre>opkg install /tmp/apn-web_1.0.3_all.ipk</pre>

Access the Interface

Open your browser and go to:

<pre>http://192.168.1.1/apn.html</pre>

# Interface Screenshots

<div style="text-align: center; margin: 20px 0;">
  <h3>Screen 1</h3>
  <img src="https://github.com/ilblogdicristiangallo/apn-web-html_ipk/blob/main/Screenshot/apn-web1.0.1-Screen.png?raw=true" alt="APN Web Interface Screen 1" width="600" style="border: 1px solid #ccc; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1);" />
  <p style="color: #555; font-size: 14px;">Initial APN selection interface (QMI, ModemManager and MBIM Cellular supported)</p>
</div>

<div style="text-align: center; margin: 20px 0;">
  <h3>Screen 2</h3>
  <img src="https://github.com/ilblogdicristiangallo/apn-web-html_ipk/blob/main/Screenshot/apn-web1.0.1-Screen2.png?raw=true" alt="APN Web Interface Screen 2" width="600" style="border: 1px solid #ccc; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1);" />
  <p style="color: #555; font-size: 14px;">APN details pre-filled with detection based on selected modem type</p>
</div>


<div style="text-align: center; margin: 20px 0;">
  <h3>Screen 3</h3>
  <img src="https://github.com/ilblogdicristiangallo/apn-web-html_ipk/blob/main/Screenshot/apn-web1.0.1-Screen3.png?raw=true" alt="APN Web Interface Screen 3" width="600" style="border: 1px solid #ccc; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1);" />

</div>
<div style="text-align: center; margin: 20px 0;">
  <h3>Screen 4</h3>
  <img src="https://github.com/ilblogdicristiangallo/apn-web-html_ipk/blob/main/Screenshot/apn-web-1.0.3-interface2.png" alt="APN Web Interface Screen 4" width="600" style="border: 1px solid #ccc; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1);" />
</div>

<div style="text-align: center; margin: 20px 0;">
  <h3>Screen 5</h3>
  <img src="https://github.com/ilblogdicristiangallo/apn-web-html_ipk/blob/main/Screenshot/apn-web-1.0.3-interface3.png?raw=true" alt="APN Web Interface Screen 5" width="600" style="border: 1px solid #ccc; border-radius: 8px; box-shadow: 0 2px 6px rgba(0,0,0,0.1);" />
  <p style="color: #555; font-size: 14px;">Final configuration confirmation with available action buttons</p>
</div>
