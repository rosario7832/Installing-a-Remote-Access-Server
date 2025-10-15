# Installing a Remote Access Server

The purpose of installing this server is to allow other devices to connect to the internet through our **Windows Server**.

**RSAT (Remote Server Administration Tools):**  
Allows you to install Active Directory tools (Active Directory Users and Computers, Group Policy Management, etc.) on a Windows 10/11 workstation and remotely manage the domain.

---

## 🔹 Installation Steps

1. Open **Server Manager Dashboard**.
2. Start the **Add Roles and Features** wizard.
3. Click *Next* until you reach **Server Roles**, then select **Remote Access**.
   <img src="https://i.imgur.com/htLOkJd.png" height="50%" width="60%"/>
4. Accept the required features.
5. In **Role Services**, select **Routing**  
   > *(by default, **DirectAccess and VPN (RAS)** will also be selected)*.
 <img src="https://i.imgur.com/F4gWiXV.png" height="50%" width="60%"/>

6. Click *Next* until you reach the installation stage.  
   ⚠️ This process may take several minutes.

---

## 🔹 Configuring Routing and Remote Access

1. After installation, go to **Tools** → **Routing and Remote Access**.
2. In the window, locate your local server, right-click it, and select:  
   **Configure and Enable Routing and Remote Access**.
3. Click *Next* → Select **NAT**  
   > This allows internal clients to connect to the internet using a public IP address.
4. On the next screen, choose:  
   **Use this public interface to connect to the Internet**  
   and select the interface connected to the internet.
 <img src="https://i.imgur.com/U4AmeOL.png" height="50%" width="60%"/>

5. Click *Next* → *Finish*.  
   ⚡ Setup may take a few moments.

---

## ✅ Verification

- Once completed, the red arrow on the **local server (DC)** icon will turn **green**.  
- New configuration options will be available.
 <img src="https://i.imgur.com/17UP3zE.png" height="50%" width="60%"/>
   

---

✔️ The remote access server is now fully configured.
