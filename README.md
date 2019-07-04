# DM-1701_RT84_MD-UV380_RT3s Codeplugs

This codeplug was originally built for the Baofeng DM-1701 and has been further enhanced, with minor modificaton, for any of the TYT type DMR handhelds which support 3000 channels and 64 channels per zone. It was converted from the MD380-90_All_AU_DMR+analog Comprehensive Australian codeplugs which was developed for the for TYT MD-380 and MD-390 as originally developed by Matt, VK2MRC for the GSTARS (Goulburn and Southern Tablelands Amateur Radio Society). Anyone building on this Codeplug or forking, please acknowledge Matt VK2MRC and Det VK2KVP

<b>Setting your own DMR ID</b>: These codeplugs will not work until you change the value in the DMR ID to your own. This is changed in the General Settings tab of your CSP. The field is labelled "Radio ID" or "Yout DMR ID" depending on which CPS you are using. 

<b>Editing Codeplugs</b> All editing was conducted with G6AMU's DMR Codeplug Editor, whilst uploaded to test transceivers using the manufacturer's CPS tool or Farnsworth's editcp. The latest version of Codeplug Editor is available from http://www.miklor.com/DMR/DMR-380-CPEditor.php and Farnsworth's editcp is available at http://github.com/dalefarnsworth/codeplug

Dale Farnworth's editcp was used to parse the codeplugs to identify invalid fields and cleanup. This is a very versatile codeplug editor which can also be used to translate codeplug formats for other devices. Linux and Windows versions aeavailable. 

N0GSG's DMR Contact Manager is another codeplug editor worthy of consideration, with support for a very wide range of radios. It is available at: http://n0gsg.com/contact-manager/

You can also edit these codeplugs using your favourite spreadsheet application. Tools to write the CSV files to codeplugs can be found at http://www.gb3gf.co.uk/downloads.html

<b>NOTE</b>Before you write these codeplugs to your radio, replace the callsign and DMR ID with your own in General settings.

    Get G6AMU's codeplug editor from http://www.miklor.com/DMR/DMR-380-CPEditor.php
    Get Farnsworth's editcp at http://github.com/dalefarnsworth/codeplug
    Get N0GSC's Contact Manager at http://n0gsg.com/contact-manager/

<b>Hotspot/Dongle Frequencies</b>: Australian band plan assigns the following 70cm frequencies for Internet gateways:

The Australian Bandplan designates 439.125 and 439.150 for digital gateways (hotspots may be considered as such devices)

    439.125
    439.150
    439.200 is assigned for digital simplex operation.

For ease of initial setup and testing, the following manufacturers' default frequencies have been set in the codeplugs from v20:

    DV4 Mini (DV4 channels): 436.000 MHz
    DV Mega (DVm channels): 431.000 MHz

For MMDVM Simplex hotspots the following frequencies have been used:

    HS-S vkdmr: 439.125 MHz
    HS-S BML 439.175

Duplex boards need a receive and transmit frequency which, like repeaters, need several MHz separation. For MMDVM Duplex boards the following frequencies have been used:

    HS_D vkdmr: Radio RX 439.95, Radio TX 432.950
    HS_D BM: Radio RX 438.95, Radio TX 431.950

<b>UHF CB Channels</b>. Australian UHF CB channels have been included, but in Read-Only mode. Note that these radios are not type approved for UHF CB transmision. If these channels are included, they must be set to Receive-only mode.

<b>Testing</b>. These codeplugs are provided "as is" without support. Use them at your own risk. They have been tested to work on a Baofeng DM-1701 running firmware v2.02

<b>Channels and Zones</b>. Explore the codeplug with your favourite CPS tool to see which zones and channels have been included. 
For each of the VK-DMR repeaters, the following channels have been included: 01 - 3801 ACT, 02 - 3802 NSW, 03 - 3803 Vic, 04 - 3804 Qld, 05 - 3805 SA, 06 - 3806 WA, 07 - 3807 Tas, 08 - 3808 NT, 09 - 3809 s1, 10 - 505 AU, 11 - 113 WW, 12 - 123 WW, 13 - 13 WWE, 14 - 3810 s1, 15 - 9 s1, 16 - 8 s1, 17 -5 s1

For MMDVM Hotspots, I have cerated four Zones "HS_S", " "HS_D". Each of these two zones include both VK-DMR (DMR+) Channels in Bank A and Brandmeister channels in Bank B. The VK-DMR channels in "HS_S" and ""HS_D" zones are configured to optimally perform with the VK-DMR network servers, as discussed by Roger Clark at https://www.rogerclark.net/new-australian-dmr-ipsc2-settings/

<b>RELEASE NOTES</b>

<b>RT3s-UV380_All_VK_DMR+analog_v20.rdt</b>
- Created zones iRBM-2RYS, 2RYS-3RGN, 2RGN-2RHR. These are included for ease of use by members of the GSTARS club for ease of use when moving between their local VK-DMR repeaters. These zones are included here as an example of how the dual banks may be used.
- Added the following DMR repeaters to include all VK-DMR repeaters as at 1 Jul 2019: VK3RBD, VK3RBQ, VK3RDR, VK3RGV, VK3 TRA, VK7RAK, VK8RDM
- A few of the analogue channels had incorrect frequency settings. These have been corrected.
- Reset GPS System to "None" for all channels
- Reset RX Group List to "None" for all channels (these transceivers do not need a RX Group entry)

