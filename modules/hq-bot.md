# HQ Bot

## Overview

The HQ system has a "bot" service that performs clean up operations on the system on a set interval \(hourly, daily, or weekly\). Over time, members may change division, or have their VATSIM account updated. By default, your account on HQ is updated each time you log in. If you do not log in within 24 hours and you are a resident member of one of the divisions that have given their Autotools access then the system will update your record automatically on a daily basis.

Any actions that are done by the HQ Bot will appear in the system log as **HQ SYSTEM \(000000\)**.

## Functions

The HQ bot performs the following functions...

* Update user information \(name, atc/pilot rating, region, division, and total atc/pilot time\) every 24 hours or whenever the user re-logs into HQ
* If the member transferred divisions \(ex: VATME to VATEUD\), the following will happen:
  * Remove the member from the Home vACC in HQ
  * Remove the "Approved For" permissions in the Home vACC
  * Remove the member from any staff positions they held
  * Remove any exam tokens assigned to the member
  * Remove Mentor status if the member was a mentor at their Home vACC
  * Revoke any TeamSpeak privilege keys assigned \(for VATME division members\)
* If the member is suspended by the network, it will also ban them from logging into HQ until they are returned back to active status \(non-suspended rating\) on VATSIM

## Transfers Out of HQ

If you transfer divisions and had a Home vACC set, you must apply to your Home vACC as a **visitor controller** once your tranfer completes. Please check your Home vACC policies for visitor controller information.

