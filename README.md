# apn-web_1.0.1_all.ipk

The apn-web.ipk package enables automatic APN configuration for all Italian mobile operators directly from a web interface, accessible via both desktop and mobile browsers.

# Description

apn-web_1.0.1_all.ipk is an OpenWrt package that provides automatic APN configuration for all Italian mobile operators through a web interface. The interface works on both desktop and mobile browsers and is designed to configure WAN connections using either the QMI protocol or ModemManager, which can now be selected directly from the apn.html page.

If the WAN interface is already configured as qmi or modemmanager (cellular), the system automatically detects the active APN and pre-fills it in the interface, making the setup even easier. Just click Apply Configuration to activate the changes.

Features

Predefined APN selector (TIM, Vodafone, WindTre, Iliad, etc.)

IP type selection: IPv4, IPv6, IPv4v6

Optional SIM PIN input

Automatic APN pre-fill if WAN is active (QMI or ModemManager)

Modem type selection: QMI or ModemManager

Buttons for:

Applying configuration (set_apn)

Restarting WAN (restart_wan)

Rebooting the router (reboot_router)

Copying selected APN

Localized success/error messages (Italian/English)

Responsive layout for smartphones and tablets

# Requirements

OpenWrt router with 4G-5G modem

QMI-compatible modem (cdc-wdm) or ModemManager-compatible modem

WAN interface configured as qmi or modemmanager

# Installation
# Method 1: WinSCP (Windows)

Connect to your router using WinSCP:

Protocol: SCP

Host: 192.168.1.1

Port: 22

Username: root

Password: (blank or your router password)

Upload the file apn-web_1.0.1_all.ipk to the /tmp directory

Open a terminal (via PuTTY or WinSCP) and run:

<pre>opkg install /tmp/apn-web_1.0.1_all.ipk</pre>

# Method 2: SCP (Linux/macOS)

Copy the file to your router:

<pre>scp apn-web_1.0.1_all.ipk root@192.168.1.1:/tmp/</pre>


SSH into the router:

<pre>ssh root@192.168.1.1</pre>


Install the package:

<pre>opkg install /tmp/apn-web_1.0.1_all.ipk</pre>

Access the Interface

Open your browser and go to:

<pre>http://192.168.1.1/apn.html</pre>

<pre>Interface Screenshots</pre>
