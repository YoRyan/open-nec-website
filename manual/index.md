---
title: Manual
layout: page
---

# Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

# Installing the mod

You can find the latest release and changelog on the [GitHub releases page](https://github.com/YoRyan/open-nec/releases). To install a release, simply copy the contents of the Zip archive's Assets\ folder into your own Train Simulator Assets\ folder, overwriting files if prompted.

If you intend to use Open NEC in combination with other mods, such as Fan Railer's enhancement packs, always install Open NEC last. This ensures that Open NEC's script files are not overwritten by versions shipped by other mods. If installing Open NEC breaks another mod in some way, we would appreciate a bug report.

# Guide to safety systems

Both the ATC and ACSES systems are present and work exactly as they do in Train Sim World's [Providence Line](https://store.steampowered.com/app/2386110/Train_Sim_World_4_Compatible_Northeast_Corridor_Boston__Providence_Route_AddOn/) and [Trenton Line](https://store.steampowered.com/app/2386170/Train_Sim_World_4_Compatible_Northeast_Corridor_New_York__Trenton/) DLC's. The ACSES positive stop function is also present and will detect upcoming stop signals, but the braking curve is enforced down to 0 mph only when driving on the [Long Island Rail Road](https://store.steampowered.com/app/1922043/Train_Simulator_Long_Island_Rail_Road_New_York__Hicksville_Route_AddOn/) route, as it is the only Train Simulator Classic DLC with the necessary signaling information included.

If you need a refresher on how these systems work, here's a guide courtesy of cActUsjUiCe:

### ACSES (maximum authorized speed of track and positive stop signals)

Acknowledgment required for all ACSES track speed downgrades at the actual start of the lower speed location, even if train is currently below new speed. Acknowledgment is not required if train accelerates over current speed or busts the braking curve down to a new lower speed.

Overspeed conditions:

- **0-3MPH over track speed and/or braking curve:** No action.
- **3-6MPH over track speed and/or braking curve:** Audible alarm only. Alarm cannot be silenced until train is brought down to less than 3MPH over track speed. Some equipment will also incur a penalty if speed is not reduced and/or suppression is not achieved within a specified time period.
- **3-6MPH over track speed and/or braking curve:** Audible alarm only. Alarm cannot be silenced until train is brought down to less than 3MPH over track speed. Some equipment will also incur a penalty if speed is not reduced and/or suppression is not achieved within a specified time period.

### ATC (cab signaling system)

Acknowledgment required for all ATC cab signal downgrades, even if train is currently below new speed.  Acknowledgment is not required if train accelerates over the current cab signal speed.

Overspeed conditions:

- **ATC cab signal downgrade:**

  ATC cab signal overspeed on a downgrade typically starts at 1MPH over limit.

  Audible alarm sounds immediately and will sound until acknowledgement *and* either train is brought under speed or suppression is obtained. If train is not brought under speed or suppression is not obtained within specified time period (6 seconds normally), a Penalty application will occur. The penalty will bring the train to a full stop if not recovered. Recovery on the fly from a penalty is possible once target speed is reached and all other conditions are met. 
- **Accelerating over ATC cab signal speed:**

  ATC cab signal overspeed while accelerating over current cab signal speed is typically starts at 1-3MPH over limit.

  Audible alarm sounds immediately and will sound until either train is brought under speed or suppression is obtained. Acknowledgement is not required. If train is not brought under speed or suppression is not obtained within specified time period (6 seconds normally), a penalty application will occur. The penalty will bring the train to a full stop if not recovered. Recovery on the fly from a penalty is possible once target speed is reached and all other conditions are met.

# Errata for individual equipment

### Amtrak EMD AEM-7

The cruise control has been fixed. To use it, turn the dial to your desired speed and set the throttle to the desired maximum amount of power.

### Amtrak Acela Express

There is a known bug with the June 4, 2020 version of Fan Railer's enhancement mod: The signal speed display on the ADU is unreadable. While you can use the signal heads to infer which aspect is being displayed, it is still impossible to distinguish between the 60 mph and 80 mph cab speeds.

### Metro-North Kawasaki M8

The automatic power change function using the P key, HUD, or Xbox controller has been removed. Instead, the pantograph control now functions as a simple power cutoff switch. To switch between power modes, you should use the in-cab "mode of operation" knob.

### Metro-North P32AC-DM

Unfortunately, some of the P32's scenarios and quick drive consists incorrectly set the P32 for diesel mode at startup--even when the scenario begins in Grand Central Terminal, or when the consist is labeled "Third Rail."

### NJ Transit Arrow III

The green speed bar is not animated correctly and always shows the vehicle's current speed. Therefore, Open NEC uses the *red* speed bar to display the maximum authorized speed.

### NJ Transit Comet IV

The green and red speed bars are missing from the ADU model. There is a gray bar, but it always shows the vehicle's current speed. Therefore, Open NEC uses the green digits on the inside of the speedometer to display the maximum authorized speed.