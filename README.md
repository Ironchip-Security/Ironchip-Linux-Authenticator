<p align="center">
  <img alt="Icon Logo" src="./assets/icon.png" width="100"/>
</p>
<h1 align="center">Ironchip</h1>

<p align="center" back>
    <a href="https://www.linux.org">
    <img alt="Latest release" src="https://shields.io/badge/linux--9cf?logo=Linux&style=social"/>
  </a>
  
  <a href="https://github.com/Ironchip-Security/Ironchip-Linux-Authenticator/releases">
    <img alt="Release" src="https://img.shields.io/github/v/release/Ironchip-Security/Ironchip-Linux-Authenticator?color=green"/>
  </a>
  
  <a href="https://github.com/Ironchip-Security/Ironchip-Linux-Authenticator/releases">
    <img alt="Release date" src="https://img.shields.io/github/release-date/Ironchip-Security/Ironchip-Linux-Authenticator?color=orange"/>
  </a>
</p>

## IDENTITY PROTECTION

Elevate your cybersecurity strategy with Ironchip Identity Platform, designed to bring the power of Multi-Factor Authentication (MFA) to your desktop computing environment. [Know more](https://www.ironchip.com/solutions/identity_platform/win-mac-linux/).

**Role-based privilege management:**
Set different user privileges. Prevents unauthorized users from accessing the rest of the system and misusing information, mitigating malicious users.

**Restrict access from unauthorized places:**
Generate enabled access from authorized areas and take your security to the next level.

**Supervision of accesses in real time:**
Check user activity, view access on a timeline, get reports and download them for full control.

**Intrusion detection system (IDS):**
Location-based reporting system to alert of sim swapping, phishing, device switching, etc.

<p align="center">
 <a href="https://www.youtube.com/watch?v=G-rr6BzcQZ0"> 
  <img alt="Logon showcase gif" src="./assets/showcase-logon.gif" alt="animated" width="550"/>
 </a>
</p>

## Download

Download the latest installer (`.deb`) version from [Release](https://github.com/Ironchip-Security/Ironchip-Linux-Authenticator/releases).

## Desktop Application

### What it is

Identity management must be nowadays considered as an essential component for security in organizations. To address this need, Ironchip provides organizations with the scalability and security necessary to offer their users a consistent experience and a reduced risk of vulnerabilities.

**Get a notification on your device**
Communication for authentication is done over a double-encrypted channel which implements a TLS plus asymmetric elliptic key encryption.

### Installing process

To install the Ironchip Authenticator into your device:

  ```bash
      sudo dpkg -i <path to .deb file >
  ```
   
 - To ensure security, you will be prompted to enter your password. This authorizes the operation and allows the installation to proceed.

 - Once the installation process is finished. All you need to do is [enroll the device](https://knowledge.ironchip.com/en/aplicaci%C3%B3n-de-escritorio#registro), and you are good to go.

### Uninstalling Application
To uninstall the application:

  ```bash
     sudo dpkg -r ironchip-authenticator
  ```

To uninstall the application from your Mac, follow these steps:

   - You will be prompted to enter your administrator password.

### How to disable USB

  **Run the Command**:
   - Type the following command in Terminal and press `Enter`:
   
     ```bash
     sudo ironchip-service configure --restrict-usb=true
     ```
   - You will be prompted to enter your administrator password.

### How to enable proxy
  Automatic Proxy: If you enable this option, the application will use the proxy configured in the system.

  **Run the Command**:
   - Type the following command in Terminal and press `Enter`:
   
     ```bash
       sudo ironchip-service configure --proxy-enable=true
     ```
     Manual Proxy: If you prefer to configure the proxy manually, the application will take the proxy details from the config.json file.

  ```bash
      sudo ironchip-service configure --proxy-manual=true --proxy-manual-uri 127.0.0.1:8080
  ```

