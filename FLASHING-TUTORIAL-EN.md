# GSI Flashing Guide (super.img)
### Requirements
- A Samsung device with unlocked bootloader.
- Odin (Windows) or Heimdall (Linux/Mac).
- The `super.img` file (GSI image).
- USB drivers for your device.
- USB cable.

### Disclaimer
[**Don't forget that all responsibility is yours.**](https://github.com/GoofyOzy4/lineage-a3core-gsi#%EF%B8%8F--disclaimer)

### Using Odin (Windows)

1. **Download and Install Odin:**
   - Obtain the latest version of Odin from a trusted source.
   - Install Samsung USB drivers on your PC.

2. **Prepare the Device:**
   - Enable `OEM Unlocking` and `USB Debugging` in Developer Options.
   - Reboot to recovery with `Volume Up` + `Power` and choose `Wipe Data`.
   - Boot your device into `Download Mode` by holding `Volume Down` + `Power`.
   - Confirm entry into Download Mode by pressing the required button on the screen.

3. **Load the Image in Odin:**
   - Open Odin on your PC.
   - Connect the device via USB. Odin should recognize it ("Added" message).
   - Repack your .img from .zip archive to .tar .
   - Click the `AP` button and select the `super.tar` file.

4. **Flash the Image:**
   - Click `Start` to begin the flashing process.
   - Wait for the process to complete. The device will reboot automatically.

5. **Verify the Flash:**
   - After the reboot, check if the GSI is successfully flashed by entering the system.

---

### Using Heimdall (Linux/Mac)

1. **Install Heimdall:**
   - Install Heimdall from your distribution’s package manager or its [official website](https://glassechidna.com.au/heimdall/).

2. **Prepare the Device:**
   - Follow the same steps as in Odin to enable `OEM Unlocking` and `USB Debugging`.
   - Wipe Data with `Recovery` as described earlier.
   - Boot into `Download Mode` as described earlier.

3. **Transfer the Image:**
   - Open a terminal and navigate to the directory containing unpacked the `super.img` file.
   - Connect your device via USB.
   - Execute the following command:
     ```
     heimdall flash --super super.img
     ```

4. **Wait for Completion:**
   - Heimdall will flash the image and provide progress updates in the terminal.
   - Once complete, the device will reboot automatically.

5. **Verify the Flash:**
   - As with Odin, check the system to ensure the GSI has been applied.
