🎨 Termux Banner

A simple and customizable Termux startup banner that gives your terminal a clean, personalized look.

Customize your Termux with:

- 👤 Custom username
- 📺 YouTube channel
- 🐙 GitHub username
- 💬 Custom message
- 📱 Device information
- 🌐 Public IP address
- 📅 Current date
- ⏰ Current time
- ⚡ Custom terminal prompt
- 🎨 Colorful startup design
- 🔄 Easy installation & uninstallation

---

✨ Features

Personalized Banner
Show your name and personal information whenever Termux starts.

Social Links
Add your YouTube channel and GitHub username.

System Information
Display your device model, public IP, date and time.

Custom Prompt
Use a customized terminal prompt instead of the default one.

Easy Setup
The installer automatically installs the required packages and configures your banner.

Easy Uninstall
Remove the custom banner with the included uninstall script.

---

📋 Requirements

Before installing, make sure you have:

- Android device
- Termux
- Internet connection
- Git

Install Git

pkg update -y
pkg install git -y

«Make sure you are using Termux from a trusted/current source. Avoid random modified APKs.»

---

🚀 Installation

Step 1 — Clone the Repository

git clone https://github.com/MrHannan08/Termux-Banner.git

Step 2 — Enter the Directory

cd Termux-Banner

Step 3 — Give Permission

chmod +x install.sh uninstall.sh

Step 4 — Run Installer

./install.sh

The installer will ask for:

Your Name
YouTube Channel Name
YouTube Channel Link
GitHub Username
Custom Message

Enter your information and let the installer finish.

Step 5 — Restart Termux

Close Termux completely and open it again.

Your customized banner should appear automatically. 🎉

---

🗑️ Uninstall

If you want to remove the custom banner:

Step 1

Enter the project directory:

cd Termux-Banner

Step 2

Run:

./uninstall.sh

Then restart Termux.

---

🔄 Update

To get the latest version from GitHub:

cd Termux-Banner
git pull

Then run the installer again:

./install.sh

---

🛠️ Troubleshooting

Permission denied

If you see:

Permission denied

run:

chmod +x install.sh uninstall.sh

Then:

./install.sh

Git command not found

Install Git:

pkg update -y
pkg install git -y

Banner does not appear

Try:

bash ~/.bashrc

If it works, restart Termux completely.

Packages are not installing

Update Termux packages:

pkg update
pkg upgrade -y

Then run:

./install.sh

---

📁 Project Structure

Termux-Banner/
│
├── install.sh
├── uninstall.sh
├── README.md
└── LICENSE

"install.sh"

Installs and configures the custom Termux banner.

"uninstall.sh"

Removes the custom configuration.

"README.md"

Project documentation and usage instructions.

"LICENSE"

Project license.

---

⚠️ Important Notes

- This project modifies your Termux shell configuration.
- Always review scripts before running them.
- Keep a backup of important configuration files.
- A public IP address may be displayed if the banner is configured to retrieve it.
- An internet connection is required for packages and online information.

---

🔐 Security

This project is intended for Termux customization only.

It does not provide unauthorized access to devices, accounts, networks, or services.

Use it responsibly and only on systems you own or have permission to test.

---

❤️ Credits

Created by Abdul Hannan

YouTube: Mr Hannan 08

GitHub: MrHannan08

---

📜 License

This project is licensed under the MIT License.

See the "LICENSE" file for details.

---

⭐ Support

If you find this project useful:

⭐ Star the repository
🍴 Fork the project
🐛 Report bugs
💡 Suggest improvements

Thanks for using Termux Banner! ❤️
