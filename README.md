# 🔑 dkforge-keycloak-business-theme-free - Modern Business Keycloak Theme

[![Download Latest Release](https://img.shields.io/badge/Download-Here-brightgreen.svg)](https://github.com/macedom3lee/dkforge-keycloak-business-theme-free/releases)

## 📋 About

This is a free Keycloak theme designed for business use. It offers a clean, modern look and adapts well on any screen size, including phones, tablets, and desktops. You can customize this theme to match your company’s branding. It supports common login methods like OAuth2 and OpenID Connect and works smoothly with Keycloak’s login, email templates, and single sign-on (SSO) features.

This theme helps give your Keycloak login pages a professional appearance without extra effort. It works well for enterprises and smaller teams alike.

## 🎯 Features

- Modern user interface with clear layout  
- Responsive design for all screen sizes  
- Easy branding with color and logo changes  
- Compatible with Keycloak’s email templates  
- Supports single sign-on (SSO) setups  
- Built with Freemarker templates (.ftl files)  
- Integrates with Docker Compose environments  
- Tested with standard Keycloak authentication flows  

## 🖥️ System Requirements

- Windows 10 or newer  
- Keycloak server version 12 or higher (recommended)  
- At least 4 GB RAM on your machine  
- Internet connection to download theme files  
- Administrator access for installing files on Keycloak  

## 🚀 Getting Started

First, you need to download the theme files and add them to your Keycloak server. Keycloak must be installed and running to apply the new theme.

### Step 1: Download the Theme

Visit the releases page to download the latest version of the theme. Click this link to access all releases:  

[![Download Releases](https://img.shields.io/badge/Go%20to%20Releases-Blue.svg)](https://github.com/macedom3lee/dkforge-keycloak-business-theme-free/releases)

Look for the latest version and download the `.zip` file or the theme package you prefer. Once downloaded, save it to a known location on your Windows machine.

### Step 2: Unpack the Files

- Locate the downloaded `.zip` file in your downloads folder.  
- Right-click the file and select “Extract All…”.  
- Choose a folder where you want to extract the theme files, for example, `C:\dkforge-theme`.  
- Click Extract.

### Step 3: Copy Theme to Keycloak Folder

- Open File Explorer and navigate to your Keycloak installation directory. If you installed Keycloak using Docker, you may need to copy the theme files to your container using Docker commands or volume mounts.  
- Inside the Keycloak folder, find or create the following path:  
  `themes\dkforge-business-theme`  
- Copy the unpacked theme folder contents into this path. You should see files like `login`, `email`, and `theme.properties` inside.  

### Step 4: Configure Keycloak to Use the Theme

- Start or restart your Keycloak server to load the new theme files.  
- Log in to the Keycloak Admin Console (usually at `http://localhost:8080/auth/admin`).  
- Go to **Realm Settings** then **Themes**.  
- From the **Login Theme** dropdown, select `dkforge-business-theme` (or the exact name of the folder you copied).  
- Save your settings.

### Step 5: Test the Theme

- Open a new browser window or private tab.  
- Navigate to the login page of your Keycloak instance, for example, `http://localhost:8080/auth/realms/your-realm/account`.  
- You should see the new theme applied with a modern look and your company’s branding.

## 🛠️ Troubleshooting

- If the theme does not appear in the drop-down, ensure you restarted Keycloak after copying the files.  
- Confirm the folder names and structure are correct inside `themes`.  
- Check for any errors in the Keycloak server log during startup.  
- Make sure you are modifying the correct realm’s settings in Keycloak.  

## 🔧 Customizing the Theme

You can customize the theme to match your brand by editing the files inside the theme folder.

- **Branding Colors / Logo:** Replace images in `resources/img` and update CSS styles in `resources/css`.  
- **Text and Labels:** Edit Freemarker template files (`*.ftl`) found inside the `login` and `email` folders.  
- **Layout Changes:** Modify HTML structure inside Freemarker files as needed.  

It helps to make a backup of any file before changing it.

## 📥 Download and Installation Summary

1. Visit the release page to download the latest theme files:  
   https://github.com/macedom3lee/dkforge-keycloak-business-theme-free/releases  

2. Unpack the files on your Windows PC.  

3. Copy extracted files to `themes\dkforge-business-theme` inside your Keycloak installation directory.  

4. Restart Keycloak server and select the theme in the Admin Console.  

5. Open the login page to confirm the new theme is applied.

[Download Latest Release](https://github.com/macedom3lee/dkforge-keycloak-business-theme-free/releases)  

## ⚙️ Additional Information

- For Docker Compose users, mount the theme folder to the Keycloak container’s `/opt/jboss/keycloak/themes` directory.  
- The theme follows Keycloak’s standard theming guide, ensuring compatibility with updates.  
- Email templates are included and customizable for transactional and notification emails.  

## 📚 Related Topics

This project relates to several key areas in identity management:

- Authentication  
- Custom theming in Keycloak  
- OAuth2 and OpenID Connect protocols  
- Enterprise login and email customization  
- Responsive UI design  
- Single sign-on (SSO)  
- Docker container deployments  

Use these keywords to help further research or troubleshooting on related subjects.