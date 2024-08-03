# Ubuntu

## Comprehensive List of Ubuntu Commands

## System Information and Management

- **Get system information:**
  ```bash
  uname -a
  ```

- **Get detailed system information:**
  ```bash
  lsb_release -a
  ```

- **List hardware information:**
  ```bash
  lshw
  ```

- **Check available disk space:**
  ```bash
  df -h
  ```

- **Check memory usage:**
  ```bash
  free -h
  ```

- **List all running processes:**
  ```bash
  ps aux
  ```

- **Get detailed information about a specific process:**
  ```bash
  ps -p <PID> -o pid,comm,%cpu,%mem,etime
  ```

- **List all installed packages:**
  ```bash
  dpkg -l
  ```

- **Check system uptime:**
  ```bash
  uptime
  ```

- **Get current date and time:**
  ```bash
  date
  ```

## File and Directory Management

- **List files and directories:**
  ```bash
  ls -la
  ```

- **Create a new directory:**
  ```bash
  mkdir directoryname
  ```

- **Delete a directory:**
  ```bash
  rm -rf directoryname
  ```

- **Copy files:**
  ```bash
  cp sourcefile destinationfile
  ```

- **Move files:**
  ```bash
  mv sourcefile destinationfile
  ```

- **Delete files:**
  ```bash
  rm filename
  ```

- **Search for files:**
  ```bash
  find /path/to/search -name filename
  ```

- **Find files containing specific text:**
  ```bash
  grep -r "searchtext" /path/to/search
  ```

- **Get file or directory size:**
  ```bash
  du -sh filename
  ```

- **Get the last modified date of a file:**
  ```bash
  stat filename
  ```

- **Rename a file:**
  ```bash
  mv oldname newname
  ```

## Network Commands

- **Ping a host:**
  ```bash
  ping hostname
  ```

- **Trace route to a host:**
  ```bash
  traceroute hostname
  ```

- **Test network connection to a port:**
  ```bash
  nc -zv hostname port
  ```

- **View routing table:**
  ```bash
  netstat -rn
  ```

- **Flush DNS cache:**
  ```bash
  sudo systemd-resolve --flush-caches
  ```

- **Display network interfaces:**
  ```bash
  ip a
  ```

- **Display network connections:**
  ```bash
  ss -tuln
  ```

- **List open ports:**
  ```bash
  sudo lsof -i -P -n
  ```

- **Show firewall rules:**
  ```bash
  sudo ufw status verbose
  ```

- **Configure a static IP address:**
  ```bash
  sudo nano /etc/netplan/01-netcfg.yaml
  ```

## User and Group Management

- **List all users:**
  ```bash
  cut -d: -f1 /etc/passwd
  ```

- **Add a new user:**
  ```bash
  sudo adduser username
  ```

- **Delete a user:**
  ```bash
  sudo deluser username
  ```

- **Add a user to a group:**
  ```bash
  sudo usermod -aG groupname username
  ```

- **Remove a user from a group:**
  ```bash
  sudo deluser username groupname
  ```

- **List all groups:**
  ```bash
  cut -d: -f1 /etc/group
  ```

## Security and Permissions

- **Check file permissions:**
  ```bash
  ls -l filename
  ```

- **Change file permissions:**
  ```bash
  chmod 755 filename
  ```

- **Change file ownership:**
  ```bash
  chown user:group filename
  ```

- **Check process usage:**
  ```bash
  top
  ```

- **Stop a process by PID:**
  ```bash
  sudo kill <PID>
  ```

- **Start a process:**
  ```bash
  ./processname
  ```

## System and Application Logs

- **View system logs:**
  ```bash
  sudo journalctl
  ```

- **View specific log entries:**
  ```bash
  sudo journalctl -u servicename
  ```

- **Clear logs:**
  ```bash
  sudo journalctl --vacuum-time=1d
  ```

- **View authentication logs:**
  ```bash
  sudo cat /var/log/auth.log
  ```

## Package Management

- **Update package list:**
  ```bash
  sudo apt update
  ```

- **Upgrade all packages:**
  ```bash
  sudo apt upgrade
  ```

- **Install a new package:**
  ```bash
  sudo apt install packagename
  ```

- **Remove a package:**
  ```bash
  sudo apt remove packagename
  ```

- **Search for a package:**
  ```bash
  apt search packagename
  ```

- **Show package details:**
  ```bash
  apt show packagename
  ```

- **Clean up package cache:**
  ```bash
  sudo apt clean
  ```

## System Maintenance

- **Run a file system check:**
  ```bash
  sudo fsck /dev/sdX
  ```

- **Update the system:**
  ```bash
  sudo apt update && sudo apt upgrade
  ```

- **Reboot the system:**
  ```bash
  sudo reboot
  ```

- **Shutdown the system:**
  ```bash
  sudo shutdown now
  ```

## Networking and System Monitoring

- **Monitor system resources:**
  ```bash
  htop
  ```

- **Check CPU usage:**
  ```bash
  mpstat
  ```

- **Monitor network traffic:**
  ```bash
  iftop
  ```

- **View disk usage:**
  ```bash
  df -h
  ```

- **Monitor disk I/O:**
  ```bash
  iostat
  ```

## Power Management

- **Check battery status:**
  ```bash
  upower -i /org/freedesktop/UPower/devices/battery_BAT0
  ```

- **Manage power settings:**
  ```bash
  sudo pm-powersave
  ```

## Summary

This list covers a broad range of Ubuntu commands for system management, file and directory handling, network diagnostics, security, user and group management, and more. These commands provide essential functionality for administering and maintaining Ubuntu systems effectively. Copy and paste these commands into your terminal as needed.
