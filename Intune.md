# Adding Devices to Intune Using Autopilot

This guide provides step-by-step instructions on how to add devices to Intune using Autopilot.

## Prerequisites

Before starting the device addition process, make sure you have the necessary permissions to access the Intune and Autopilot services on your Microsoft 365 account.

## Steps

1. **Obtain Device Information**

   You'll need your device's hardware ID. This can be obtained using the `Get-WindowsAutoPilotInfo` script from PowerShell.

2. **Add Device in Intune**

   Log into the [Microsoft Endpoint Manager admin center](https://endpoint.microsoft.com/).

   - Navigate to `Devices` > `Enroll devices` > `Windows enrollment`.
   - Under `Windows Autopilot Deployment Program`, choose `Devices`.
   - Select `+ Create` to add a new device.
   - Upload the .csv file with the hardware ID you obtained earlier.

3. **Assign a Deployment Profile**

   - Navigate to `Devices` > `Windows` > `Windows enrollment` > `Deployment Profiles`.
   - Assign a deployment profile to the device.

4. **Sync the Device**

   The device will now sync with Intune. If the device is already set up, you'll need to reset it to trigger the Autopilot process.

Please note that the process might vary slightly depending on your Microsoft 365 environment setup.

For additional details, refer to the official Microsoft documentation.
