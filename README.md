# RTL8812AU Wi-Fi Driver Installation

This guide provides the necessary steps to compile and install the `rtl8812au` driver for Debian/Ubuntu-based systems.

## 🚀 Installation

Run the following commands to update your system, install the required dependencies, and build the driver via DKMS:

```bash
# 1. Update the package information
sudo apt update

# 2. Install DKMS and Git
sudo apt install dkms git

# 3. Install build dependencies
sudo apt install build-essential libelf-dev linux-headers-$(uname -r)

# 4. Download the driver files using Git
git clone [https://github.com/aircrack-ng/rtl8812au.git](https://github.com/aircrack-ng/rtl8812au.git)

# 5. Navigate to the downloaded directory
cd rtl8812au

# 6. Install the driver
sudo make dkms_install
