
```bash name=termux-setup.sh
#!/bin/bash

# Termux setup script

# Update and upgrade packages
pkg update && pkg upgrade -y

# Install common packages
pkg install -y git curl wget

# Set up custom Termux configurations
mkdir -p ~/.termux

# Copy custom configuration files
cp -r .termux/* ~/.termux/

echo "Termux setup completed!"
