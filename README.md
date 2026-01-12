macOS Tahoe on Dell OptiPlex 3050 Micro
![4218](https://github.com/user-attachments/assets/0fd34a68-e237-4128-9666-33320c799ddf)

A complete installation guide and EFI for running macOS Tahoe on the Dell OptiPlex 3050 Micro.

> ⚠️ Important: This guide is for macOS Tahoe (final release) — not Tahoe Beta.
The installer must be Tahoe 26.2, otherwise the installation will not work.

---

📦 Creating the macOS Tahoe USB Installer

1️⃣ Download macOS Tahoe Installer (26.2)

Download the macOS Tahoe Vanilla image from Olarila:

🔗 https://olarila.com/topic/6278-olarila-vanilla-images-macos-installer/

Make sure the version is Tahoe 26.2.


---

2️⃣ Flash the Image to a USB Drive

Option A: Balena Etcher (Recommended)

Download Balena Etcher: 🔗 https://etcher.balena.io/

Flash the downloaded macOS Tahoe image to your USB drive.

Option B: Win32 Disk Imager (If Etcher Fails)

If Etcher fails, use Win32 Disk Imager instead:

🔗 https://win32diskimager.org/

⚠️ Important note:
You will not see the image file by default.
In File Explorer, change the file filter to “All Images” to select the installer file.


---

3️⃣ Assign a Drive Letter to the EFI Partition

1. Download MiniTool Partition Wizard: 🔗 https://www.partitionwizard.com/


2. Open MiniTool Partition Wizard


3. Locate the USB’s EFI partition


4. Assign it a drive letter of your choice (it will usually be “None” by default)




---

4️⃣ Copy the EFI Folder

1. Download the EFI folder provided in the Releases section


2. Open Explorer++ as Administrator


3. Open the EFI partition you just mounted


4. Delete any existing EFI folder


5. Copy my EFI folder into the EFI partition




---

5️⃣ Boot and Install

Boot from the USB drive

Follow the macOS installer

Install macOS Tahoe on the Dell OptiPlex 3050 Micro



---

🖥 System Information

Desktop Model: Dell OptiPlex 3050 Micro

Images of the PC specifications are included.

Hardware Specifications

CPU: Intel® Core™ i3-7100T (3.4 GHz)

GPU: Intel HD Graphics 630

RAM: 4 GB

Storage: SSD

Optical Drive: Not present



---

🖥 Graphics & Display

HDMI: Fully working

DisplayPort: Not tested

VGA: Not supported



---

🔊 Audio

Audio does not work natively.
Audio is functional using VoodooHDA.

Tutorials used:

https://olarila.com/topic/42836-easy-audio-solution-on-hackintosh-on-macos-tahoe/

https://olarila.com/topic/43796-macos-tahoe-audio-fix/#google_vignette



---

🔌 USB Ports

USB ports are already mapped in the provided EFI

If USB does not work correctly on your system, you must map them manually


USB mapping guide: 🔗 https://olarila.com/topic/14220-hackintosh-usb-port-mapping-guide-2023/


---

⚙️ BIOS Settings

Configure the BIOS exactly as follows:

SATA Operation: AHCI

Fastboot: Thorough

Integrated NIC: Enabled

Secure Boot: Disabled

Absolute: Disabled

TPM 2.0 Security: On

Intel SGX: Enabled

UEFI Network Stack: Enabled



---

🧩 Bluetooth

Status: Not working

If anyone manages to get Bluetooth working on this system, please let me know.



---

🧪 Notes & Support

This setup is for macOS Tahoe (final release) — not Tahoe Beta

If you encounter any issues with the EFI, please report them so improvements can be made
