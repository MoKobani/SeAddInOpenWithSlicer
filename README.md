# SeAddInOpenWithSlicer
 A Solid Edge Add-In that exports the active Part, Sheet Metal, or Assembly document as an STL file
  with a single click and automatically opens it in a configurable 3D printing slicer (e.g., Bambu Studio).

  ## Features

  The Add-In adds a new ribbon tab **"Mojo Smart Solutions"** to Solid Edge, containing the group
  **"3D-Printing"**. It provides two buttons:

  | Button | Function |
  |---|---|
  | **Open in Slicer** | Saves the active Part, Sheet Metal, or Assembly document as an STL file in the user's temp
  folder and opens it directly in the configured slicer. |
  | **Select Slicer** | Opens a file dialog to select and save the path to the desired slicer's .exe file. |


  Supported Solid Edge document types: `.par` (Part), `.psm` (Sheet Metal), `.asm` (Assembly).

  ## Requirements

  - Solid Edge (with the SolidEdgeCommunity framework installed)
  - .NET Framework 4.8
  - An installed 3D printing slicer (e.g., Bambu Studio, PrusaSlicer, Cura, …)
  - Administrator rights for registering the Add-In

  ## Installation

  1. **Download:** Download the repository/release as a ZIP file from GitHub.
  2. **Unzip:** Extract the ZIP file.
  3. **Save:** Save the extracted folder locally – ideally directly in the folder where Solid Edge
     is installed (e.g., `C:\Program Files\Siemens\...`).
  4. **Close Solid Edge:** Solid Edge must be completely closed before registration.
  5. **Run Install.bat as Administrator:** Right-click `Install.bat` and select
     **"Run as administrator"**.
  6. **Make a selection:** In the menu that appears, choose the option that matches your installed
     Solid Edge/Windows version:

     [Options]
     1 Register (Solid Edge x86)
     2 Unregister (Solid Edge x86)
     3 Register (Solid Edge x64)
     4 Unregister (Solid Edge x64)
     5 Quit

  - **Option 3 (x64)** for the now-standard 64-bit installation of Solid Edge on 64-bit Windows.
  - **Option 1 (x86)** only if a 32-bit version of Solid Edge is in use.

  If in doubt, you can check the bitness of Solid Edge via *Help → About Solid Edge*.
  7. Start Solid Edge – the new "Mojo Smart Solutions" ribbon tab should now be visible.

  ## Uninstallation

  Run `Install.bat` again as Administrator and choose the matching **Unregister** option
  (2 for x86 or 4 for x64).


  ## Author

  Created by Dipl.-Ing. Mohammad Hassan
