sunnypilot - Version 0.8.14-1 (2022-06-26)
========================
* sunnypilot 0.8.14 release - based on openpilot 0.8.14 devel
* "0.8.14-prod-c3" branch only supports comma three
  * If you have a comma two, EON, or other devices than a comma three, visit sunnyhaibin's discord server for more details: https://discord.gg/wRW3meAgtx
* Mono-branch support
  * Honda/Acura
  * Hyundai/Kia/Genesis
  * Toyota/Lexus
  * Volkswagen MQB
* Modified Assistive Driving Safety (MADS) Mode
  * NEW❗: CRUISE (MAIN) now engages MADS for all supported car makes
  * NEW❗: Added toggle to disable disengaging Automatic Lane Centering (ALC) on the brake pedal
* Dynamic Lane Profile (DLP)
* NEW❗: Gap Adjust Cruise (GAC)
  * openpilot longitudinal cars can now adjust between the lead car's following distance gap via 3 modes:
    * Steering Wheel (SW) | User Interface (UI) | Steering Wheel + User Interface (SW+UI)
* NEW❗: Custom Camera & Path Offsets
* NEW❗: Torque Lateral Control from openpilot 0.8.15 master (as of 2022-06-15)
* NEW❗: Torque Lateral Control Live Tune Menu
* NEW❗: Speed Limit Sign from openpilot 0.8.15 master (as of 2022-06-22)
* NEW❗: Mapbox Speed Limit data will now be utilized in Speed Limit Control (SLC)
  * Speed limit data will be utilized in the following availability:
    * Mapbox (active navigation) -> OpenStreetMap -> Car Interface (Toyota's TSR)
* Custom Stock Longitudinal Control
  * NEW❗: Volkswagen MQB
  * Honda
  * Hyundai/Kia/Genesis
* NEW❗: Mapbox navigation support for non-Prime users
  * Visit sunnyhaibin's discord server for more details: https://discord.gg/wRW3meAgtx
* Hyundai/Kia/Genesis
  * NEW❗: Enhanced SCC (ESCC) Support
    * Requires hardware modification. Visit sunnyhaibin's discord server for more details: https://discord.gg/wRW3meAgtx
  * NEW❗: Smart MDPS (SMDPS) Support - Auto-detection
    * Requires hardware modification and custom firmware for the SMDPS. Visit sunnyhaibin's discord server for more details: https://discord.gg/wRW3meAgtx
* Toyota/Lexus
  * NEW❗: Added toggle to enforce stock longitudinal control

sunnypilot - Version 0.8.12-4 (2022-04-09)
========================
* Note: Each supported car make has additional updates. Please check the changelogs of relevant car make branches for in-depth changelogs
* NEW❗: Roll Compensation and SteerRatio fix from comma's 0.8.13
* NEW❗: Dev UI to display different metrics on screen
  * Click on the "MAX" box on the top left of the openpilot display to toggle different metrics display
  * Lead car relative distance; Lead car relative speed; Actual steering degree; Desired steering degree; Engine RPM; Longitudinal acceleration; Lead car actual speed; EPS torque; Current altitude; Compass direction
* NEW❗: Stand Still Timer to display time spent at a stop with M.A.D.S engaged (i.e., stop lights, stop signs, traffic congestions)
* NEW❗: Current car speed text turns red when the car is braking
* NEW❗: Export GPS tracks into GPX files and upload to OSM thanks to eFini!
* NEW❗: Enable ACC and M.A.D.S with a single press of the RES+/SET- button
* NEW❗: Dedicated icon to show the status of M.A.D.S.
* NEW❗: No Offroad Fix for non-official devices that cannot shut down after the car is turned off
* FIXED: MADS button unintentionally set MAX when using stock longitudinal control thanks to Spektor56!

sunnypilot - Version 0.8.12-3
========================
* NEW❗: Bypass "System Malfunction" alert toggle
  * Prevent openpilot from returning the "System Malfunction" alert that hinders the ability use openpilot

sunnypilot - Version 0.8.12-2
========================
* NEW❗: Disable M.A.D.S. toggle to disable the beloved M.A.D.S. feature
  * Enable Stock openpilot engagement/disengagement
* ADJUST: Initialize Driving Screen Off Brightness at 50%

sunnypilot - Version 0.8.12-1
========================
* sunnypilot 0.8.12 release - based on openpilot 0.8.12 devel
* Dedicated Hyundai/Kia/Genesis, Honda, Subaru, Toyota branch support
  * Subaru: Based on subaru-community thanks to martinl!
* NEW❗: OpenStreetMap integration thanks to the Move Fast team!
  * NEW❗: Vision-based Turn Control
  * NEW❗: Map-Data-based Turn Control
  * NEW❗: Speed Limit Control w/ optional Speed Limit Offset
  * NEW❗: OpenStreetMap integration debug UI
  * Only available to openpilot longitudinal enabled cars
* NEW❗: Hands on Wheel Monitoring according to EU r079r4e regulation
* NEW❗: Disable Onroad Uploads for data-limited Wi-Fi hotspots when using OpenStreetMap related features
* NEW❗: Fast Boot (Prebuilt)
* NEW❗: Auto Lane Change Timer
* NEW❗: Screen Brightness Control (Global)
* NEW❗: Driving Screen Off Timer
* NEW❗: Driving Screen Off Brightness (%)
* NEW❗: Max Time Offroad
* Improved user feedback with M.A.D.S. operations thanks to Spektor56!
  * Lane Path
    * Green🟢 (Laneful), Red🔴 (Laneless): M.A.D.S. engaged
    * White⚪: M.A.D.S. suspended or disengaged
    * Black⚫: M.A.D.S. engaged, steering is being manually override by user
  * Screen border now only illuminates Green when SCC/ACC is engaged

sunnypilot - Version 0.8.10-1 (Unreleased)
========================
* sunnypilot 0.8.10 release - based on openpilot 0.8.10 `devel`
* Add Toyota cars to Force Car Recognition

sunnypilot - Version 0.8.9-4
========================
* Hyundai: Fix Ioniq Hybrid signals

sunnypilot - Version 0.8.9-3
========================
* Update home screen brand and version structure

sunnypilot - Version 0.8.9-2
========================
* Added additional Sonata Hybrid Firmware Versions
* Features
    * Modified Assistive Driving Safety (MADS) Mode
    * Dynamic Lane Profile (DLP)
    * Quiet Drive 🤫
    * Force Car Recognition (FCR)
    * PID Controller: add kd into the stock PID controller

sunnypilot - Version 0.8.9-1
========================
* First changelog!
* Features
    * Modified Assistive Driving Safety (MADS) Mode
    * Dynamic Lane Profile (DLP)
    * Quiet Drive 🤫
    * Force Car Recognition (FCR)
    * PID Controller: add kd into the stock PID controller
