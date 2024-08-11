# Installing and Updating Drivers
 
In this guide, you will learn how to download or update drivers on your computer.

::: warning
It is highly recommended to avoid using third-party software to update or install your drivers.
:::

## Identifying Your Hardware

The first step in installing drivers is to correctly identify the hardware you need drivers for. This information can be found in your computer's manual or by using the Device Manager. You can access the device manager by right-clicking the Windows start button or by pressing <kbd>Win</kbd> + <kbd>X</kbd> and selecting Device Manager. In the Device Manager, look for the device you require drivers for, and expand its entry to see its model number.

You can also use the System Information tool to find hardware information; open System Information, navigate to the “Hardware” section and find the device you require drivers for.

## Method 1: Using Windows Update

You can usually find drivers for your devices in Windows Update, instead of having to manually download the file.

1. Open Settings via the start menu or by pressing <kbd>Win</kbd> + <kbd>I</kbd>.
 
2. Go to Update & Security (on Windows 10) or Windows Update (on Windows 11).
 
3. Click on “Check for Updates” or "Download & Install Updates".
 

Windows Update might say that you are up-to-date, even if optional updates are available. You can check for additional optional updates in the 'Optional updates' section of Windows Update settings.

On Windows 11:

1. Click "Advanced options".

   ![Windows 11's Windows Update settings, with the Advanced options button highlighted.](./img/installing-and-updating-drivers/optional-updates/windows-update-advanced-options.png)

2. Click "Optional updates".

   ![The Advanced options menu, with the Optional updates button highlighted.](./img/installing-and-updating-drivers/optional-updates/windows-update-advanced-options-optional-updates.png)

3. Click "Driver updates" to show the list of available driver updates, if there are any.

   ![The Optional updates menu, with the Driver updates menu highlighted.](./img/installing-and-updating-drivers/optional-updates/windows-update-optional-updates-driver-updates.png)

4. Select any optional updates you wish to install, then click "Download & install".

   ![An available optional driver update, with the Download & install button selected.](./img/installing-and-updating-drivers/optional-updates/windows-update-driver-update-example.png)

On Windows 10, a "View optional updates" link will appear under "Check for updates" if optional updates are available. Click on it to see the list of available driver updates.

## Method 2: Using your OEM's website

::: tip Note
"OEM" here refers to the manufacturer of an entire device, like a laptop or pre-built desktop. If you are using a custom-built computer, you should follow [Method 3](#method-3-using-your-manufacturer-s-website) instead.
:::

It is highly recommended to download or update your drivers through your manufacturer's website, as that will guarantee proper functionality, provided you've installed the correct drivers. This is especially a good idea for your Graphics Card (GPU) Drivers.

All you need to do is:
1. On the search engine of your choice (Google, Bing, etc…), search for "{device manufacturer} drivers".
2. Visit the manufacturer's website and enter the model of your device, then follow the instructions on the page.
3. When you select the product, you may be shown with 2 options:
	- Download the driver downloader (recommended).
	- Download this specific driver only and install manually.

### Well-known manufacturers' websites

- [Dell](https://www.dell.com/support/home/en-us?app=drivers)
 
- [HP](https://support.hp.com/us-en/drivers)
 
- [Lenovo](https://pcsupport.lenovo.com/us/en)

- [ASUS](https://www.asus.com/support/download-center)


## Method 3: Using your manufacturer's website

::: tip Note
"Manufacturer" here refers to the manufacturer of an individual piece of hardware. If you are using a laptop or a pre-built desktop, you should probably download drivers from your OEM's website instead. See [Method 2](#method-2-using-your-oem-s-website).
:::

For each piece of hardware in your computer that you wish to get drivers for:
1. On the search engine of your choice (Google, Bing, etc…), search for "{hardware manufacturer} drivers".
 
2. Search for the model number of the piece of hardware you want to upgrade/install drivers for.
 
3. When you select the product, you may have two options:
 
    - Download the driver downloader (recommended).
    - Download this specific driver only and install manually.


See [Reinstalling GPU drivers from the OEM's website](reinstalling-gpu-drivers#method-3-oem-website) for more information on installing GPU drivers.

## Troubleshooting 🔧

### If you can access Windows:

<br />

#### Verifying Driver Signatures

Verifying driver signatures ensures you are installing secure, untampered and correct drivers issued by your hardware manufacturer.

1. Press <kbd>Win</kbd> + <kbd>R</kbd>, then type in `sigverif` and press <kbd>Enter</kbd>.

2. A window will pop up. Press the `Start` button to verify driver signatures.

#### Updating Drivers with Device Manager

1. Press <kbd>Win</kbd> + <kbd>X</kbd> and then clicking the "Device Manager" option. You can also search for it in the Start Menu.

   ![The Win+X 'power user' menu, with Device Manager highlighted.](./img/installing-and-updating-drivers/troubleshooting/device-manager-power-user-menu.png)

2. In Device Manager, find the device that is causing problems (you might have to expand a category), right-click on it, and click "Properties".

   ![The context menu for a display adapter in Device Manager, with Properties highlighted.](./img/installing-and-updating-drivers/troubleshooting/device-manager-properties-button.png)

3. Go to the "Driver" tab at the top of the window, and then click "Roll Back Driver".

   ![The properties window for a device in Device Manager, with the Driver tab and Roll Back Driver button highlighted.](./img/installing-and-updating-drivers/troubleshooting/device-manager-properties-roll-back-driver.png)

4. Windows will ask you why you're rolling back to a previous driver. Select a reason, and click "Yes". If you want to, you can leave a detailed response in the "Tell Us More" field, at the bottom of the window.

   ![The confirmation dialogue presented after selecting Roll Back Driver.](./img/installing-and-updating-drivers/troubleshooting/driver-rollback-confirmation.png)

5. Windows will then restore your driver to the previous version, which could take up to 5-10 minutes.

   ![The prompt to restart your computer, shown after rolling back a driver.](./img/installing-and-updating-drivers/troubleshooting/hardware-change-restart-prompt.png)

### Safe Mode
Safe mode is a diagnostic tool, which loads Windows with only the essential drivers. This allows you to access Windows even if the problematic driver is causing issues during normal boot.

1. Enter Safe Mode:

   **On Windows 10 or 11:**

   1. Open the Start menu, click on the power button, and hold <kbd>Shift</kbd> while clicking Restart. This will take you to the Windows Recovery Environment.


   2. Click on "Troubleshoot"

      ![A screenshot showing the Windows Recovery Environment screen with an arrow pointing at the Troubleshoot button.](./img/installing-and-updating-drivers/winre/choose_an_option_screen.png)

   3. Then, select "Advanced options"

      ![A screenshot of the Troubleshooting menu in the Windows Recovery Environment with the Advanced Options button highlighted.](./img/installing-and-updating-drivers/winre/troubleshoot_screen.png)

   4. Finally, click "Startup Settings" and then "Restart".

      ![A screenshot of the Advanced Options menu in the Windows Recovery Environment, with the Startup Settings button highlighted.](./img/installing-and-updating-drivers/winre/advanced_options_screen.png)

   After your computer restarts, press <kbd>4</kbd> to boot into Safe Mode, or <kbd>5</kbd> to boot into Safe Mode with internet access.

   **On earlier versions of Windows:**

   - Restart your computer and repeatedly press F8 before the Windows logo appears.
   - At the Advanced Boot Options menu, select “Safe Mode” to boot into Safe Mode, or “Safe Mode with Networking” to boot into Safe Mode with internet access.

2. Uninstall the Driver in Safe Mode:

   Once in safe mode, you can uninstall the problematic driver:

   1. Open the Device Manager (search for it in the Start Menu).

   2. Expand the category for the device with the recently installed driver.

      ![The context menu for a display adapter in Device Manager, with Properties highlighted.](./img/installing-and-updating-drivers/troubleshooting/device-manager-properties-button.png)

   3. In Device Manager, find the device that is causing problems (you might have to expand a category), right-click on it, and click "Properties".

      ![The properties window for a device in Device Manager, with the Driver tab and Roll Back Driver button highlighted.](./img/installing-and-updating-drivers/troubleshooting/device-manager-properties-roll-back-driver.png)

   4. Go to the "Driver" tab at the top of the window, and then click "Roll Back Driver".

      ![The confirmation dialogue presented after selecting Roll Back Driver.](./img/installing-and-updating-drivers/troubleshooting/driver-rollback-confirmation.png)

   5. Windows will ask you why you're rolling back to a previous driver. Select a reason, and click "Yes". If you want to, you can leave a detailed response in the "Tell Us More" field, at the bottom of the window.

      ![The confirmation dialogue presented after selecting Roll Back Driver.](./img/installing-and-updating-drivers/troubleshooting/driver-rollback-confirmation.png)

   6. Windows will then restore your driver to the previous version, which could take up to 5-10 minutes.

      ![The prompt to restart your computer, shown after rolling back a driver.](./img/installing-and-updating-drivers/troubleshooting/hardware-change-restart-prompt.png)


Or if you can't access the normal safe mode, you may try and access Safe Mode with Command Prompt and execute the following commands in Command Prompt (replace `not_working_driver` with the driver that isn't working):

```
DISM /Image:C:\ /Get-Drivers
DISM /Image:C:\ /Remove-Driver /Driver:not_working_driver.inf
```

3. You should see something like this:  
```
Found 1 driver package(s) to remove.
Removing 1 of 1 – not_working_driver.inf: The driver package was successfully removed.
The operation completed successfully.
```

1. At startup options, click Troubleshoot.

   ![Screen showing advanced startup options, titled "Choose an option".](./img/installing-and-updating-drivers/winre/choose_an_option_screen.png)

2. Then, click on "Advanced Options"

   ![The Windows Recovery Environment's troubleshoot screen.](./img/installing-and-updating-drivers/winre/troubleshoot_screen.png)

3. Finally, click on "System Restore" and follow the instructions

   ![Screen in the Windows Recovery Environment, titled "Advanced options", with the option "System Restore" highlighted.](./img/installing-and-updating-drivers/winre/advanced_options_screen.png)

### Startup Repair
    
   1. Select "Troubleshoot"

      ![Screen showing advanced startup options, titled "Choose an option".](./img/installing-and-updating-drivers/winre/choose_an_option_screen.png)
    
   2. Select "Advanced options"
    
      ![The Windows Recovery Environment's troubleshoot screen.](./img/installing-and-updating-drivers/winre/troubleshoot_screen.png)
    
   3. Select "Startup Repair"
    
      ![Screen in the Windows Recovery Environment, titled "Advanced options".](./img/installing-and-updating-drivers/winre/advanced_options_screen.png)

### Reinstall Windows

If none of the solutions above work, you may need to reinstall Windows. This will erase all your data and applications, so make sure you have a backup. You can learn how to backup your data [here](/wiki/backup.html).

You can learn how to download and reinstall Windows [here](downloading-windows).