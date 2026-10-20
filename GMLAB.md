# Piper calibration UI source

This is a formal fork of agilexrobotics/Piper_sdk_ui. The hardware/piper-linker
branch preserves the local joint-window change: expose the existing individual
Set Zero and All Set Zero controls and allocate their layout column.

Set Zero changes encoder calibration and can disable joints. These controls are
not normal teleoperation commands. The change has only been syntax checked;
no CAN interface was opened and no hardware calibration was performed.

PrometheusV4 hardware/piper-linker pins this source as an optional reference
dependency. It is not registered as a second live robot owner or automatically
launched by any workflow. Use the maintained Prometheus operator entry for live
hardware tasks.
