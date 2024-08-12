# If-your-Ubuntu-system-isn-t-displaying-a-graphical-user-interface-GUI-
If your Ubuntu system isn't displaying a graphical user interface (GUI), you might be in a terminal-only session. Here’s how to troubleshoot and get your GUI back:

1. **Check if the GUI is installed:**
   Run the following command to see if the GUI packages are installed:
   ```bash
   sudo apt-get install ubuntu-desktop
   ```

2. **Start the GUI manually:**
   Try starting the display manager with:
   ```bash
   sudo systemctl start gdm3
   ```
   Replace `gdm3` with `lightdm` or `sddm` if you’re using a different display manager.

3. **Check for errors:**
   Check the status of the display manager to see if there are any errors:
   ```bash
   sudo systemctl status gdm3
   ```

4. **Reboot:**
   Sometimes a simple reboot can fix GUI issues:
   ```bash
   sudo reboot
   ```

5. **Check for Updates:**
   Ensure your system is up-to-date:
   ```bash
   sudo apt-get update
   sudo apt-get upgrade
   ```

If these steps don’t resolve the issue, there might be more specific problems with your system configuration or graphics drivers
