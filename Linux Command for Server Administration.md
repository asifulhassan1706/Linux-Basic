
# Linux Server Administration Commands

Below is a comprehensive list of Linux commands frequently used in server administration, with comments on where and why you would use them.

## 1. User and Permission Management

```bash
# Add a new user (useful for creating separate accounts)
sudo adduser <username>

# Delete a user
sudo deluser <username>

# Change password for a user
sudo passwd <username>

# Add user to a group (e.g., sudo group)
sudo usermod -aG <groupname username>

# Show current user
whoami

# Show currently logged-in users
who
```

## 2. File and Directory Operations

```bash
# List files (detailed view)
ls -l

# Change directory
cd /path/to/directory

# Copy files
cp source destination

# Move or rename files
mv source destination

# Remove file
rm filename

# Remove directory recursively
rm -rf <directoryname>

# Create a new directory
mkdir <directoryname>

# Show current path
pwd

# Find a file or directory
find /path/to/search -name <filename>
```

## 3. File Viewing and Editing

```bash
# View file content
cat <filename>

# View file content page by page
less <filename>

# View first lines of a file
head <filename>

# View last lines of a file (useful for logs)
tail <filename>

# View log file in real-time
tail -f /var/log/syslog

# Edit file with nano editor
nano <filename>

# Edit file with vim editor
vim <filename>
```

## 4. Disk and Filesystem Management

```bash
# Show disk usage
df -h

# Show directory size
du -sh /path/to/directory

# Mount a filesystem
sudo mount /dev/sdX /mnt

# Unmount a filesystem
sudo umount /mnt

# Check disk usage of all directories
sudo du -ah / | sort -rh | head -n 20
```

## 5. Process and Service Management

```bash
# Show running processes
ps aux

# Real-time process monitoring (CPU/memory)
top

# Advanced real-time process monitoring
htop

# Kill a process by PID
kill PID

# Kill a process by name
pkill <processname>

# Start a service (systemd)
sudo systemctl start <servicename>

# Stop a service
sudo systemctl stop <servicename>

# Restart a service
sudo systemctl restart <servicename>

# Check service status
sudo systemctl status <servicename>

# Enable service to start at boot
sudo systemctl enable <servicename>

# Disable service at boot
sudo systemctl disable <servicename>
```

## 6. Network Management

```bash
# Show IP address of server
ip a

# Show routing table
ip route

# Test connectivity to host
ping host

# Check open ports (needs net-tools or ss)
netstat -tulnp   # or ss -tulnp

# Download file from URL
wget <URL>

# Download file using curl
curl -O <URL>

# SSH into another server
ssh <user@host>

# Secure copy files to/from server
scp file <user@host:/path>

# Show active network connections
ss -ltnp
```

## 7. Package Management (Debian/Ubuntu)

```bash
# Update package list
sudo apt update

# Upgrade all packages
sudo apt upgrade -y

# Install a package
sudo apt install <packagename> -y

# Remove a package
sudo apt remove <packagename> -y

# Search for a package
apt search keyword
```

## 8. Logs and Monitoring

```bash
# View system logs
journalctl

# View logs for a specific service
journalctl -u <servicename>

# Check last system reboot time
who -b

# Show system uptime
uptime
```

## 9. Compression and Archiving

```bash
# Create a tar archive
tar -cvf <archive.tar> directory/

# Extract a tar archive
tar -xvf <archive.tar>

# Create a compressed tar archive
tar -czvf <archive.tar.gz> directory/

# Extract compressed tar archive
tar -xzvf <archive.tar.gz>
```

## 10. Security and Firewall

```bash
# Change file permissions
chmod 755 <filename>

# Change file ownership
chown user:group <filename>

# Check firewall status (ufw)
sudo ufw status

# Allow a port through firewall
sudo ufw allow 22

# Deny a port through firewall
sudo ufw deny 22

# Enable firewall
sudo ufw enable

# Disable firewall
sudo ufw disable
```

## 11. System Information

```bash
# Show system information
uname -a

# Show CPU information
lscpu

# Show memory usage
free -h

# Show block devices
lsblk

# Show OS release info
cat /etc/os-release
```
