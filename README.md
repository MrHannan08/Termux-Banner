# ⚡ Termux-Banner

<p align="center">
  <b>Custom Termux Banner Installer</b>
</p>

<p align="center">
  A simple Bash-based tool to create a personalized and colorful startup banner for Termux.
</p>

---

## 📖 Overview

**Termux-Banner** is a Bash-based customization tool designed for **Termux on Android**.

It automatically creates a personalized startup banner by configuring the user's `~/.bashrc` file.

During installation, you can enter your own name, YouTube channel, GitHub username and custom message. The banner can also display useful system information such as your device model, public IP address, current date and current time.

The goal of this project is to make Termux more personal, attractive and easier to customize without manually writing the entire Bash configuration yourself.

---

## ✨ Features

- 🎨 Colorful startup banner
- 👤 Custom username
- 📺 YouTube channel name
- 🔗 YouTube channel link
- 🐙 GitHub username
- 💬 Custom extra message
- 📱 Automatic device model detection
- 🌐 Public IP display
- 📅 Current date
- ⏰ Current time
- ⚡ Custom Bash prompt
- 🔧 Automatic package installation
- 🖥️ Automatic `.bashrc` configuration
- 🗑️ Easy uninstall script
- 📱 Termux / Android focused
- 🚀 Simple interactive setup

---

## 🎯 Benefits

### 🎨 Personalize Your Termux

Add your own name, social links and custom message to the Termux startup screen.

### ⚡ Easy Setup

The installer automatically handles the main configuration instead of requiring you to manually create the banner.

### 🧑‍💻 Beginner Friendly

The installer asks simple questions and uses your answers to configure the banner.

### 📱 Made for Termux

The project is designed around the Termux environment on Android.

### 🔄 Easy Removal

The included `Uninstall.sh` script restores the default Termux Bash configuration.

---

## 📋 Requirements

You need:

- Android device
- Termux
- Internet connection
- Git

For the best experience, use an up-to-date Termux installation.

---

# 🚀 Installation

## 1. Update Termux

Open Termux and run:

```bash
pkg update -y
pkg upgrade -y
```

---

## 2. Install Git

```bash
pkg install git -y
```

---

## 3. Clone the Repository

```bash
git clone https://github.com/MrHannan08/Termux-Banner.git
```

---

## 4. Enter the Project Directory

```bash
cd Termux-Banner
```

---

## 5. Check the Files

```bash
ls
```

The repository should contain files such as:

```text
install.sh
Uninstall.sh
README.md
```

---

## 6. Give Permission to the Installer

```bash
chmod +x install.sh
```

---

## 7. Run the Installer

```bash
bash install.sh
```

You can also run:

```bash
./install.sh
```

---

# ⚙️ Interactive Setup

When `install.sh` starts, it asks for your personal information.

## 👤 1. Your Name

The installer asks:

```text
[?] Apna Naam Likhein:
➜
```

Enter the name you want to display.

Example:

```text
Mr Hannan
```

---

## 📺 2. YouTube Channel Name

The installer asks:

```text
[?] Apna YouTube Channel Name Likhein:
➜
```

Example:

```text
Mr Hannan 08
```

---

## 🔗 3. YouTube Channel Link

The installer asks:

```text
[?] Apna YouTube Channel Link Likhein:
➜
```

Example:

```text
https://youtube.com/@MrHannan08
```

---

## 🐙 4. GitHub Username

The installer asks:

```text
[?] Apna GitHub Username Likhein:
➜
```

Example:

```text
MrHannan08
```

---

## 💬 5. Extra Message

The installer asks:

```text
[?] Koi Extra Message?
➜
```

You can enter any short message.

Example:

```text
Stay Anonymous
```

Or:

```text
Ethical Hacking & Cyber Security
```

---

# 🔧 Default Values

If you leave a field empty, the installer uses these default values:

```text
Name          → Hacker
Channel Name  → YouTube
Channel Link  → https://youtube.com
GitHub        → GitHub
Extra Message → Stay Anonymous
```

You can simply press **Enter** if you want to use the default value.

---

# 📦 Required Packages

The installer uses the following command-line tools:

```text
figlet
toilet
ruby
lolcat
cmatrix
neofetch
curl
```

These tools are used for:

- ASCII text
- Colorful terminal output
- Terminal customization
- System information
- Public IP lookup
- Terminal effects

The installer attempts to install the required packages automatically.

---

# 🖥️ Banner Information

After installation, the banner can display information similar to:

```text
👤 User        : Mr Hannan
📺 YouTube     : Mr Hannan 08
🔗 Link        : https://youtube.com/@MrHannan08
🐙 GitHub      : MrHannan08
💬 Message     : Stay Anonymous
📱 Device      : Your Device
🌐 IP          : Your Public IP
📅 Date        : Current Date
⏰ Time        : Current Time
```

The actual information depends on what you enter during installation and what information is available on your device.

---

# 🎨 Custom Terminal Prompt

The installer also creates a customized Bash prompt.

The prompt includes:

- Your configured username
- Current working directory
- Custom terminal colors

This gives the shell a personalized appearance instead of the standard Bash prompt.

---

# 🔄 Restart Termux

After the installation is complete, the script tells you to restart Termux.

Close Termux completely and open it again.

The customized banner should appear when the Bash shell starts.

---

# 🧠 How It Works

The basic workflow is:

```text
Start Termux
     │
     ▼
Run Install.sh
     │
     ▼
Enter Your Information
     │
     ▼
Install Required Packages
     │
     ▼
Create ~/.bashrc
     │
     ▼
Replace Configuration Placeholders
     │
     ▼
Restart Termux
     │
     ▼
Custom Banner Appears
```

The main configuration file used by the installer is:

```text
~/.bashrc
```

Bash loads this configuration when the shell starts.

---

# 📄 Install.sh

`Install.sh` is the main installation script.

It performs the following operations:

1. Clears the terminal.
2. Displays the project banner.
3. Collects user information.
4. Applies default values when fields are empty.
5. Updates Termux packages.
6. Installs required packages.
7. Creates a customized `~/.bashrc`.
8. Replaces configuration placeholders with user information.
9. Installs additional terminal tools.
10. Displays installation completion information.

---

# 📄 Uninstall.sh

`Uninstall.sh` is used to remove the customized banner.

It removes the current:

```text
~/.bashrc
```

and restores the default Termux Bash configuration from:

```text
/data/data/com.termux/files/usr/etc/bash.bashrc
```

After running the script, restart Termux.

---

# 🗑️ Uninstall

To remove the custom banner, enter the project directory:

```bash
cd Termux-Banner
```

Give permission to the uninstall script:

```bash
chmod +x Uninstall.sh
```

Run the uninstaller:

```bash
bash Uninstall.sh
```

Or:

```bash
./Uninstall.sh
```

The script will display:

```text
Uninstalled! Restart Termux.
```

Now close Termux completely and open it again.

---

# ⚠️ Backup Before Uninstalling

The current `Uninstall.sh` removes:

```text
~/.bashrc
```

If you have your own Bash settings, aliases or custom commands in that file, create a backup first:

```bash
cp ~/.bashrc ~/.bashrc.backup
```

This keeps a copy of your current configuration.

---

# 🔄 Manual Restore

You can manually restore the default Termux Bash configuration with:

```bash
rm -rf ~/.bashrc
cp /data/data/com.termux/files/usr/etc/bash.bashrc ~/.bashrc
```

Then restart Termux.

---

# 🛠️ Useful Commands

## Update Termux

```bash
pkg update -y
pkg upgrade -y
```

## Install Git

```bash
pkg install git -y
```

## Clone Repository

```bash
git clone https://github.com/MrHannan08/Termux-Banner.git
```

## Enter Project

```bash
cd Termux-Banner
```

## List Files

```bash
ls
```

## Installer Permission

```bash
chmod +x Install.sh
```

## Run Installer

```bash
bash Install.sh
```

## Uninstaller Permission

```bash
chmod +x Uninstall.sh
```

## Run Uninstaller

```bash
bash Uninstall.sh
```

## View `.bashrc`

```bash
cat ~/.bashrc
```

## Edit `.bashrc`

```bash
nano ~/.bashrc
```

## Backup `.bashrc`

```bash
cp ~/.bashrc ~/.bashrc.backup
```

---

# 🧪 Troubleshooting

## Git Is Not Installed

If you see:

```text
git: command not found
```

Run:

```bash
pkg update -y
pkg install git -y
```

Then clone the repository again.

---

## Permission Denied

If you get a permission error:

```bash
chmod +x Install.sh
```

Then run:

```bash
./Install.sh
```

For the uninstall script:

```bash
chmod +x Uninstall.sh
```

Then:

```bash
./Uninstall.sh
```

---

## Banner Does Not Appear

First, completely close and reopen Termux.

Then check whether `.bashrc` exists:

```bash
ls -la ~
```

Check its contents:

```bash
cat ~/.bashrc
```

You can also start a new Bash session:

```bash
bash
```

---

## Package Installation Problem

Update the Termux package repositories:

```bash
pkg update -y
pkg upgrade -y
```

You can also install the main tools manually:

```bash
pkg install figlet toilet ruby curl -y
```

Then install `lolcat`:

```bash
gem install lolcat
```

---

# 🌐 Public IP

The banner uses the following command to retrieve the public IP address:

```bash
curl -s ifconfig.me
```

If the device is offline or the service cannot be reached, the banner displays:

```text
Offline
```

The public IP shown by the banner is your internet-facing address, not your local/private network address.

---

# 🔐 Security & Privacy

Termux-Banner is primarily a terminal customization project.

The generated banner may display:

- Public IP address
- Device model
- YouTube information
- GitHub username
- Custom messages

Be careful when sharing screenshots of your Termux terminal.

Do not enter sensitive information such as:

```text
Passwords
API keys
Private tokens
Authentication credentials
Private account information
```

---

# 🎓 Educational Use

This project can be useful for learning:

- Bash scripting
- Shell variables
- User input
- Default values
- ANSI terminal colors
- `.bashrc` configuration
- Linux shell environments
- Termux customization
- Package management
- Command execution
- Basic shell automation
- Terminal interface design

Some Bash concepts demonstrated by this project include:

```bash
read
echo
variables
sed
cat
command substitution
file redirection
environment configuration
```

---

# 📚 Learning Opportunities

By studying this project, beginners can practice:

```text
Bash scripting
Linux shell basics
Termux configuration
Shell variables
User input handling
Text processing
Package management
Terminal customization
Command execution
Basic automation
```

The project can also serve as a small example of how a Bash script can automate configuration tasks in a Termux environment.

---

# 📂 Project Structure

```text
Termux-Banner/
│
├── Install.sh
├── Uninstall.sh
└── README.md
```

### Install.sh

Main installer responsible for creating the custom banner and configuring `.bashrc`.

### Uninstall.sh

Removes the customized Bash configuration and restores the default configuration.

### README.md

Complete project documentation.

---

# ⚠️ Termux Notes

Some commands and system information may behave differently depending on:

- Android version
- Termux version
- Device model
- Internet connection
- Installed packages
- User permissions

The project is intended for the Termux environment.

---

# ⚠️ Responsible Use

Termux-Banner is intended for:

- Personal customization
- Educational purposes
- Bash learning
- Termux experimentation
- Terminal personalization

Use the project responsibly and only on devices and environments where you have permission to make changes.

This project is a terminal customization utility and is not intended to provide unauthorized access to systems, accounts or networks.

---

# 🤝 Contributing

Contributions are welcome.

If you want to improve the project:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Test the changes in Termux.
5. Commit your changes.
6. Push the branch.
7. Open a Pull Request.

Example:

```bash
git checkout -b feature/improvement
```

After making your changes:

```bash
git add .
```

```bash
git commit -m "Improve Termux banner"
```

```bash
git push origin feature/improvement
```

Then create a Pull Request on GitHub.

---

# 🐛 Reporting Issues

If you find a bug, open an issue in the GitHub repository.

When reporting an issue, include:

- Android version
- Termux version
- Error message
- Command used
- Relevant terminal output

Do not include passwords, API keys, tokens or other sensitive information.

---

# ⭐ Support

If you find **Termux-Banner** useful, consider supporting the project:

- ⭐ Star the repository
- 🍴 Fork the project
- 🐛 Report bugs
- 💡 Suggest improvements
- 📢 Share the project

Your support helps the project grow.

---

# 👨‍💻 Author

## Abdul Hannan

**GitHub:**  
https://github.com/MrHannan08

**YouTube:**  
https://youtube.com/@MrHannan08

**WhatsApp Channel:**  
https://whatsapp.com/channel/0029VbDlP9S4NVioPURej51w

---

# 📜 License

This repository includes a `LICENSE` file.

See the `LICENSE` file in the repository for the complete license terms.

---

# ❤️ Credits

Created with ❤️ by **Abdul Hannan**

**GitHub:** MrHannan08

---

<p align="center">

## ⚡ Termux-Banner

### Customize Your Terminal. Make It Yours.

**Built for Termux • Powered by Bash • Created by MrHannan08**

⭐ Star the repository if you find it useful!

</p>
