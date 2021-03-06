---
title: Samsung SyncThru Printer
description: Instructions on how to integrate a Samsung printer providing SyncThru within Home Assistant.
ha_category:
  - System Monitor
ha_iot_class: Local Polling
ha_release: 0.66
ha_config_flow: true
ha_codeowners:
  - '@nielstron'
ha_domain: syncthru
---

The Samsung SyncThru Printer platform allows you to read current data from your local Samsung printer.

It usually provides information about the device's state, the left amount of ink or toner and the state of paper trays.

## Configuration

Go to **Configuration** >> **Integrations** in the UI, click the button with `+` sign and from the list of integrations select **Samsung SyncThru Printer**.

If your printer is on and you have enabled [SSDP](/integrations/ssdp/) discovery, it's likely that the printer is automatically discovered. In that case, you shouldn't need any information to complete configuration - simply confirm that the information displayed is correct.

The following information is displayed in separate sensors, if it is available:

 - Black, cyan, magenta and yellow toner fill level
 - Black, cyan, magenta and yellow drum state
 - First to fifth paper input tray state
 - First to sixth paper output tray state

<div class="note warning">
Note that this component or parts thereof may not work if the language of your printer is not configured to be English.
</div>
