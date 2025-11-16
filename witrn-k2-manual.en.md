# WITRN K2 Unofficial User Manual English

<a href="https://www.witrn.com/?p=2105"><img alt="WITRN K2 official homepage" src="https://img.shields.io/badge/WITRN-K2-blue"></a> <a href="https://www.witrn.com/witrn/K2/K2_V4.6.zip"><img alt="Firmware download link" src="https://img.shields.io/badge/Firmware-V4.6-blue"></a>

## Table of contents

- [1 Introduction to the Witrn K2](#introduction-to-the-witrn-k2)
- [2 Power on/screen on](#power-onscreen-on)
- [3 Power](#power)
- [4 Fast charging protocol detection and spoofing](#fast-charging-protocol-detection-and-spoofing)
- [5 Watch faces](#watch-faces)
- [6 E-Marker](#e-markers)
- [7 Firmware](#firmware)
- [8 Host computer](#host-computer)
- [9 Cable resistance](#cable-resistance)

## Information regarding this manual

This quick reference manual is **unofficial**. All content is subject to the [WITRN K2 Official Instruction Manual](https://www.witrn.com/?p=2105).

This quick reference manual aims to assist first-time users of the WITRN K2 meter. It includes frequently asked questions, and you can quickly jump to your desired question using the table of contents above, or browse through the entire manual. Unfamiliar terms are explained by their respective footnotes[^1]. This version of the manual has been translated from https://github.com/JohnScotttt/WITRN-K2-Quick-Reference-Manual . If you want to contribute in its original language, see that repository. If you want to contribute to the English translation, please submit a pull request at https://github.com/ipftalabua/WITRN-K2-Quick-Reference-Manual . The HTML version of the English manual has been created with [StackEdit](https://stackedit.io/) .

<div style="page-break-before: always;"></div>

## 1 Introduction to the Witrn K2

### Table of contents

- [1.1 Three ports](#three-ports)
- [1.2 Four buttons](#four-buttons)
- [1.3 First screen](#first-screen)
- [1.4 Second screen](#second-screen)
- [1.5 Third screen](#third-screen)
- [1.6 Fourth screen](#fourth-screen)

### 1.1 Three ports

![Three Ports](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/3ports.png)

**Type-C male connector:** Can be connected to a mobile phone or charger socket

**Type-C female connector:** Can be connected to a charging cable

**HID/NTC port:** Can be connected to a charging cable for independent power supply or to a host computer[^2] (which also acts as a power supply) or to a temperature probe (NTC)

**Note:** The correct orientation for the K2 is **from left to right** or **from right to left** as shown in the diagram. The HID connector only supplies power to the K2 itself and is not used when the K2 is used as a power meter.

### 1.2 Four buttons

+ **`BACK`**: Back button/exit
+ **`-`**: Short press: previous screen/adjust lower
  `DFU` (long press on `-`): power on and enter DFU upgrade mode
+ **`OK`**: Confirm/execute/save/enter
+ **`+`**: Short press: next screen/adjust higher
  `🗲` (long press on `+` for the lightning bolt): power on and draw power from power delivery (PD) adapters

### 1.3 First Screen

![P1_desc](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/P1_desc.png)

+ **`BACK`**
  (short press) to lock/unlock screen rotation
  (long press) to rotate the screen while locked
+ **`OK`**
  (short press) to view the PDO[^3] and RDO[^4] list (if any), see image below
  (long press) to change the screen refresh rate

![PDO&RDO](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/PDO&RDO.png)

### 1.4 Second Screen

![P2_desc](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/P2_desc.png)

+ **`BACK`**
  (short press) to switch the recording group (1 or 2 in the green title line of the screen)
+ **`OK`**
  (short press) to save MAX and AVG values
  (long press) to clear the energy and capacity records and the MAX and AVG values of the current group

### 1.5 Third Screen

![P3_desc](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/P3_desc.png)

Short press **`OK`** to change the sampling frequency.

### 1.6 Fourth Screen

![P4](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/P4.png)

+ **Fast Charge:** Enters the fast charging protocol detection screen
+ **Tools:** Enters the tools screen
+ **Lock Direction:** Locks and unlocks the screen rotation
+ **Set:** Enters the settings screen

<div style="page-break-before: always;"></div>

## 2 Power-on/screen-on

### Table of contents
- [2.1 How to power on](#how-to-power-on)
- [2.2 Why doesn't the screen light up when plugged in?](#why-doesnt-the-screen-light-up-when-plugged-in)
- [2.3 Screen remains dark when pressing the lightning bolt button during plug-in](#screen-remains-dark-when-pressing-the-lightning-bolt-button-during-plug-in)
- [2.4 Why does the screen go dark when the phone is unplugged?](#why-does-the-screen-go-dark-when-the-phone-is-unplugged)
- [2.5 Why does the K2 display "K2 DFU"?](#why-does-the-k2-display-k2-dfu)

### 2.1 How to power on

Both the left and right type-C connectors on the K2 can be used for supplying power. To power on and wake the screen, either connect a USB-C data cable to the device’s female port, or plug the K2’s built-in male connector into a power adapter.

**Note:** Regardless of the type of cable (USB-A to USB-C, short A/C, or USB-C to USB-C, short C/C) it is recommended that the button **`+`** is long pressed while connecting the K2 to a power source. This activates power delivery (PD) mode of the K2.

![how_to_open](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/how_to_open.png)

**Remark:**
> The K2 official website provides another way to power on: Press **`OK`** to power on. However, this method has limitations and is generally not recommended.
>
> When using the K2 as a charging monitor it does not need to be powered-on; it is enough to simply connect the devices. Powering it on may result in extremely slow charging and protocol errors may emerge; see [3.5 Why is the charging power so low after connecting the K2?](#35-Why is the charging power so low after connecting the K2?).

### 2.2 Why doesn't the screen light up when plugged in?

First, check if your data cable is plugged into a powered outlet.

Second, there is a chance that your charger only supplies power if the power delivery (PD) handshake has been performed. In that case, also connect a phone or another device to use the K2 as a pass-through meter[^5]. If you want to use the K2 stand-alone, the following solution may work for you.

**Solution:** The K2 uses an electronic switch. Press and hold **`+`** to activate power delivery (PD) 5V power supply; this will power on the device and light up the screen. For PD chargers it makes no difference whether pressing and holding **`+`** is performed before or after plugging the cable into the charger.

### 2.3 Screen remains dark when pressing the lightning bolt button during plug-in

Because the PD chip only connects to one set of the power pins in USB-C to USB-C (C/C) cables and C/C charging cables have two sets of power pins, there is a 50% chance that PD 5V cannot be activated.

**Solution:** Flip the charging cable at one end and repeat the power-on operation.

### 2.4 Why does the screen go dark when the phone is unplugged?

The K2 is a pass-through meter[^5] by design. If the phone was previously charging using the PD protocol, unplugging the phone will interrupt communication. In this case, the PD charger will no longer supply power and the K2 will go dark.

**Solution:** Refer to the solution for [2.2 Why doesn't the screen light up when plugged in?](#why-doesnt-the-screen-light-up-when-plugged-in)

### 2.5 Why does the K2 display "K2 DFU"?

The button **`-`** was pressed while powering on, thus entering DFU mode[^6].

**Solution:** Do not press the `-` button while powering on. Refer to [2.1 How to power on](#how-to-power-on).

<div style="page-break-before: always;"></div>

## 3 Power

### Table of contents

- [3.1 With no device plugged in, why is the power value non-zero?](#with-no-device-plugged-in-why-is-the-power-value-non-zero)
- [3.2 Why is the power displayed lower than the charger's nominal value?](#why-is-the-power-displayed-lower-than-the-chargers-nominal-value)
- [3.3 Why is the first screen showing multiple power values?](#why-is-the-first-screen-showing-multiple-power-values)
- [3.4 Why is the power value in the green/gray box in the lower right corner of the first screen different from the power supported by my phone?](#why-is-the-power-value-in-the-greengray-box-in-the-lower-right-corner-of-the-first-screen-different-from-the-power-supported-by-my-phone)
- [3.5 Why is the charging power very low after connecting the K2?](#why-is-the-charging-power-very-low-after-connecting-the-k2)

### 3.1 With no device plugged in, why is the power value non-zero?

When the K2 is connected at its female connector it will monitor its own power consumption, resulting in a power value of approximately 0.3W.

**Solution:** Using the HID port or its male connector will prevent the K2 from monitoring its own power consumption.

### 3.2 Why is the power displayed lower than the charger's nominal value?

The charger's nominal power value is its maximum power. The power actually delivered depends on how much power the attached device (e.g. phone) requests and its charging status. It is normal that the power displayed by the K2 is less than or equal to the charger's nominal power value.

### 3.3 Why is the first screen showing multiple power values?

![P1_desc](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/P1_desc.png)

A power value shown in the green box on the first screen is the maximum power as indicated by the PD power supply.

The power, voltage, and current values in the gray box at the bottom of the screen are either inferred from inductive monitoring (in case of PD power supplies) or are pseudo-values derived from the protocol (as it is the case for some proprietary protocols). They generally denote the maximum current and voltage values for the currently requested power level. The actual current and voltage readings in the center of the screen are also affected by cable voltage drop and the current state of the attached device (e.g. phone). Usually, the values displayed by the K2 should always be less than or equal to the requested values. However, for proprietary protocols there may be inference errors; this is a bug in the firmware of the K2 and will probably be fixed in a future firmware version.

### 3.4 Why is the power value in the green/gray box in the lower right corner of the first screen different from the power supported by my phone?

The answer is the same as above, i.e. it is likely that a proprietary protocol is used and the displayed values are inferred. In this case, a future firmware version may address this issue.

Some protocols also involve communication pin issues. In this case, try flipping one end of the USB-C cable and try again.

### 3.5 Why is the charging power very low after connecting the K2?

If the device (e.g. phone) makes use of fast charging and it is almost fully charged, this is normal behaviour. Refer to [3.2 Why is the power displayed lower than the charger's nominal value?](#why-is-the-power-displayed-lower-than-the-chargers-nominal-value).

If your device is capable of fast charging but fails activate it when the K2 is connected, then you probably first pressed and held the **`+`** button while connecting the K2 to the charging cable, and only after that you connected the K2 to the device/phone. In this case, the K2 is recognized as a device on its own, it does not fully act in pass-through mode. The charging adapter is communicating with the K2 and not the device/phone, causing the problem.

**Solution:** Disconnect the K2 from the power supply, then connect it again without pressing any buttons. Wait for the device/phone and charging adapter to complete the handshake. If the handshake still fails, try disconnecting and reconnecting all cables.

<div style="page-break-before: always;"></div>

## 4 Fast charging protocol detection and spoofing

### Table of contents

- [4.1 Fast charging protocols](#fast-charging-protocols)
- [4.2 Testing fast charging protocols](#testing-fast-charging-protocols)
- [4.3 Spoofing fast charging protocols](#spoofing-fast-charging-protocols)
- [4.4 Why does the screen go dark when testing fast charging protocols?](#why-does-the-screen-go-dark-when-testing-fast-charging-protocols)
- [4.5 Why can't I connect my device while performing protocol detection?](#why-cant-i-connect-my-device-while-performing-protocol-detection)
- [4.6 Can high-power fast charging be forced by protocol spoofing?](#can-high-power-fast-charging-be-forced-by-protocol-spoofing)
- [4.7 Can the charging adapter's Protocol A be changed to Protocol B by protocol spoofing?](#can-the-charging-adapters-protocol-a-be-changed-to-protocol-b-by-protocol-spoofing)
- [4.8 Why is the detected protocol different from the label on the charger?](#why-is-the-detected-protocol-different-from-the-label-on-the-charger)
- [4.9 Why is the protocol displayed in the lower right corner of the first screen different from the actual protocol on the phone?](#why-is-the-protocol-displayed-in-the-lower-right-corner-of-the-first-screen-different-from-the-actual-protocol-on-the-phone)
- [4.10 What is "PD speedup"?](#what-is-pd-speedup)
- [4.11 How to block protocols?](#how-to-block-protocols)

### 4.1 Fast charging protocols

Due to various historical issues, different mobile phone/device manufacturers have different solutions for high-power charging, each solution being a protocol. Third-party charger manufacturers communicate with the mobile phone/device to determine which solution it uses, confirming the required protocol before supplying power. These protocols are not interoperable. If the fast charging protocol provided by the charger does not match the fast charging protocol supported by the mobile phone/device, only the standard voltage of 5V will be supplied.

### 4.2 Testing fast charging protocols

**WARNING:** Do not connect a device at any stage of fast charging protocol detection or spoofing! Ignoring this warning may destroy the device! If you are an expert in this field and know exactly what you are doing, proceed.

Connect the components as shown in the diagram below and use the correct power-on method (see [2.1 How to power on](#how-to-power-on)) to start the K2. Go to the Fourth screen and select the option **Fast Charge**.

![FClist](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/ADFC_pic.png)

There is an automatic protocol detection option and several fast charging protocol spoofing options. Selecting **Automatic Protocol Detection** will bring up a prompt.

![ADFC](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/ADFC.png)

The interface varies slightly between versions. Versions v2.9 and below can only be set to detect the virtual E-Marker[^7]. To be able to change the E-Marker, go to **Set -> Virtual EMark**. Versions v3.1 and above allow quick setting of the virtual E-Marker. Version v3.4 additionally adds a "PD speedup"[^8] switch.

+ **OFF:** Indicates that virtual E-Mark data is not used.
+ **[inbuilt emark]:** Indicates that the K2's built-in default 240W (50V 5A PD3.1 EPR) virtual E-Mark data is used.
+ **[copied Emark \*NG]:** Indicates that copied E-Mark data is used. **\*NG indicates that no data has been copied**, the absence of the NG characters indicates that data has been copied.

The K2 also supports modifying virtual E-Markers by using the host software. Added E-Markers will also also be shown in this interface and can be selected. See [6.4 How to export and import E-Markers](#how-to-export-and-import-e-markers) for details.

Now, what is the most appropriate E-Marker setting? If using the original data cable (see the **Note** text below), select OFF. If not using the original data cable or using a data cable without an E-Marker, select the virtual E-Marker and press **`OK`** to enter automatic detection. After several restarts, the detection ends when END is displayed in the upper right corner.

**Note:** Although the K2 supports the virtual E-Marker[^7], the optimal detection method is to connect the K2 female connector using the official original data cable from the charger, or to connect the K2 male connector to the charger with the female connector inserted into the charger's official original data cable **with the other end loose**[^9] (used for the charger to detect the E-Marker of the data cable). The detected protocol is most accurate in this case ("PD speedup"[^8] can be selected as needed). If you are not using the original data cable, or your data cable does not have an E-Marker, select the virtual E-Marker as needed. The automatic detection protocol cannot be powered by HID. In special cases such as a black screen or an infinitely rebooting charger or power bank, HID power can be used to complete the test. During the test, the K2 will **reboot**, which is normal. The automatic detection protocol, combined with custom cables and OFF mode, can also be used to detect whether a cable supports a certain protocol.

![ADFC_result](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/ADFC_result.png)

After detection of the E-Marker is finished, you can view a list of all protocols supported by the charger. If it supports PD, press **`OK`** to view the PDO list.

The lower left corner displays the currently used E-Marker. If it is OFF, it displays "Fast Charging Protocol Detection".

For firmware versions 3.4 and above, the PD speedup[^8] switch will be displayed as ON or OFF within the green box at the top.

**Notes:**
+ The K2 auto-detection interface currently **does not detect** some modified charging protocols, only general-purpose charging protocols.
+ There are many types of modified charging protocols, see the following examples.
+ **OPPO:**
  + OPPO's outdated second-generation SVOOC (modified PPS) is **not detected**.
  + OPPO has now fully upgraded to the third-generation SVOOC (modified UFCS). The auto-detection interface does not detect these, but you can activate the third-generation SVOOC UFCS modification through the UFCS spoof menu.
+ **Xiaomi:**
  + Xiaomi's 140W, 210W, and some 67W models are special MIPPS and **are not detected**.
  + Xiaomi MIPPS only detects standard 120W or lower Xiaomi MIPPS.
+ **VIVO:**
  + The VFC protocol auto-detection menu can detect these.
  + Activating specific voltage and current can be done by entering the VFC spoof menu separately.
+ **Huawei:**
  + SCP: Currently, Huawei's main fast charging protocol is called SCP. The automatic detection can detect it.

### 4.3 Spoofing fast charging protocols

**WARNING:** Do not connect a device at any stage of fast charging protocol detection or spoofing! Ignoring this warning may destroy the device! If you are an expert in this field and know exactly what you are doing, proceed.

Selecting a fast charging protocol from the list of fast charging protocols will check whether the charging adapter supports that protocol. If that is the case, a spoofing screen is shown where voltage can be adjusted. If supported, also the current can be adjusted.

### 4.4 Why does the screen go dark when testing fast charging protocols?

A wrong power-on method has been used. For example, using **`OK`** to power on will result in a black screen when testing any fast charging protocol.

**Solution:** Pay attention to the power-on method. Refer to [2.1 How to power on](#how-to-power-on) for more details.

### 4.5 Why can't I connect my device while performing protocol detection?

**WARNING:** Do not connect a device at any stage of fast charging protocol detection or spoofing! Ignoring this warning may destroy the device! If you are an expert in this field and know exactly what you are doing, proceed.

During protocol detection the output will carry high voltages. There is a high probability that attached devices cannot handly (all of) these high voltages. Hence, both the attached device (e.g. phone) and the spoofing interface (charger, K2) will very likely be destroyed.

### 4.6 Can high-power fast charging be forced by protocol spoofing?

**WARNING:** Do not connect a device at any stage of fast charging protocol detection or spoofing! Ignoring this warning may destroy the device! If you are an expert in this field and know exactly what you are doing, proceed.

**No**, charging usually requires a handshake. Forcing higher power modes will trigger device protection at best; at worst, it will destroy the device.

### 4.7 Can the charging adapter's Protocol A be changed to Protocol B by protocol spoofing?

**WARNING:** Do not connect a device at any stage of fast charging protocol detection or spoofing! Ignoring this warning may destroy the device! If you are an expert in this field and know exactly what you are doing, proceed.

**No**, with spoofing the K2 only changes voltage and current of the output, no protocol conversion is performed. Without a proper handshake between charger and device such spoofing will trigger device protection at best; at worst, it will destroy the device.

For protocol conversion a **bridge cable** is needed. Such a cable can for example be purchased on Taobao.

### 4.8 Why is the detected protocol different from the label on the charger?

If the K2 is not connected using the official charging cable from the charger, or if the virtual E-Marker is not enabled, the K2 will not be able to detect fast charging protocols above 3A. In this case, the detected protocol will be inconsistent with the charger label. Also, the handshake protocol actually used to charge the device with this charging cable will be consistent with the one detected by the K2, meaning that fast charging will not be used.

**Solution:** Use the charger's original charging cable or a charging cable that the charger can recognize.

### 4.9 Why is the protocol displayed in the lower right corner of the first screen different from the actual protocol on the phone?

The lower right corner of the first screen displays values from monitoring the power delivery (PD) handshake or pseudo-values from protocol inference, the latter of which may be incorrect. In this case, a future firmware update may address this issue.

Some protocols also involve communication pin issues. In this case, try flipping one end of the USB-C cable and try again.

### 4.10 What is "PD speedup"?

**Note:** The official documentation lacks a good definition for "PD speedup". Hence, its explanation in this manual is solely based on some test results.

The PD speedup switch is an option in firmware version 3.4 and above. Versions below 3.4 enable PD speedup by default. The official manual says:

> "PD speedup" function: Please disable for regular charging adapters.
>
> Enable for some Apple PD charging adapters (PD speedup is only required for some Apple chargers).
>
> "PD speedup" is enabled for reading the serial number of some Apple PD charging adapters.

Generally speaking, PD speedup is only used for automatic protocol detection and reading the PD power code for Apple chargers. However, tests suggest that some non-Apple chargers may also be affected. If you encounter problems with protocol detection in firmware version 3.4 or above, try enabling or disabling PD speedup and then try again.

### 4.11 How to block protocols

Starting from firmware version 3.1, the K2 supports D+D- blocking. This can be useful for blocking protocols such as UFCS and SCP (which make use of D+D-), thus prioritizing PPS.

Go to the Fourth screen -> **Set** -> **Block D+D- lines**, select to enable or disable. The setting will take effect immediately.

<div style="page-break-before: always;"></div>

## 5. Watch faces

### Table of contents

- [5.1 How to customize watch faces and the boot screen?](#how-to-customize-watch-faces-and-the-boot-screen)
- [5.2 Why is the uploaded watch face not displayed?](#why-is-the-uploaded-watch-face-not-displayed)
- [5.3 Why does the watch face screen show "No Theme Parameters"?](#why-does-the-watch-face-screen-show-no-theme-parameters)
- [5.4 Why does the watch face screen display "No Theme Image"?](#why-does-the-watch-face-screen-display-no-theme-image)

### 5.1 How to customize watch faces and the boot screen?

**Note:** Please [upgrade the K2 firmware](https://www.witrn.com/?p=2105) to at least version v2.9

Download the [dial editing software](https://www.witrn.com/witrn/K2/K2Picture_1.1.zip) from the [official website](https://www.witrn.com/?p=2615). Unpack the archive and run `K2Picture.exe` (only Windows systems are supported). The software requires the .NET Core runtime library which should be downloaded if missing.

![k2picture](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/k2picture.png)

**Note:** Before each update the K2 must be put into DFU mode[^6].

For updating follow these steps:
- To update the **boot image**, enter DFU mode, click ① to load the image data, click ② to update the image data, and wait for the progress bar to complete.
- To update a **watch face**, enter DFU mode, click ③ to load the image data, click ④ to update the data, wait for the progress bar to complete, then enter DFU mode again, click ⑤ to import watch face parameters, click ⑥ to update parameters, and wait for the progress bar to complete.

**Note:**  The watch face will only work after both the **image** and the **parameters** have been set. They only work in tandem.

To create your own boot image or watch face, please use a 235x235 BMP for the boot image and a 240x240 BMP for the watch face. The text size and font are not the actual display font size; the text position can be adjusted by dragging. There is no preview for icon colors. After adjusting the parameters, remember to click "Save Parameters" to generate a parameter file for future use.

### 5.2 Why is the uploaded watch face not displayed?

The custom watch face is off by default: To use it, you need to enable it in the settings menu.

**Solution:** Fourth Screen -> **Set** -> **Theme screen**, enable it.

### 5.3 Why does the watch face screen show "No Theme Parameters"?

The watch face parameters are missing.

**Solution:** Upload the parameters through the watch face editing software. See [5.1 How to customize watch faces and the boot screen?](#how-to-customize-watch-faces-and-the-boot-screen) for details.

### 5.4 Why does the watch face screen display "No Theme Image"?

The watch face image is missing.

**Solution:** Upload a watch face image using watch face editing software.  See [5.1 How to customize watch faces and the boot screen?](#how-to-customize-watch-faces-and-the-boot-screen) for details.

<div style="page-break-before: always;"></div>

## 6 E-Markers

### Table of contents

- [6.1 Introduction to E-Markers](#introduction-to-e-markers)
- [6.2 What is "inbuilt emark"?](#what-is-inbuilt-emark)
- [6.3 How to read an E-Marker](#how-to-read-an-e-marker)
- [6.4 How to export and import E-Markers](#how-to-export-and-import-e-markers)

### 6.1 Introduction to E-Markers

An E-Marker is a chip embedded in a USB Type-C cable, essentially an "electronic ID card" for the cable. It declares the cable's capabilities (such as whether it supports high-speed transmission, maximum voltage and current, length, etc.) to the host and device, thereby ensuring the safety and compatibility of PD fast charging and data transmission. Cables without an E-Marker cannot support currents greater than 3A or high-speed modes.

Each manufacturer has its own E-Marker tag. Some fast charging protocols rely on E-Marker certification; without an E-Marker or with an incompatible E-Marker the handshake protocol cannot be established.

The K2 has a built-in virtual E-Marker, which can simulate the capabilities of an E-Marker to some extent, but it cannot completely replace an E-Marker. This is because some manufacturers' E-Markers are encrypted, making it impossible for the virtual E-Marker to simulate them. Furthermore, some chargers have E-Marker reading capabilities exceeding the K2's simulation capabilities, making them unrecognizable.

### 6.2 What is "inbuilt emark"?

The K2 has a default 240W (50V 5A PD3.1 EPR) virtual E-Mark tag built-in.

### 6.3 How to read an E-Marker?

The K2 has the ability to read and copy E-Markers. Connect the components as shown in the image below. Select Fourth screen -> **Tools** -> **E-Marker** to access the interface.

![read_Emark](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/read_Emark.png)

Plug the data cable into the Type-C female connector, leaving the other end loose[^9]. This will allow you to read the E-Marker information.

![Emark](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/Emark.png)

E-Marker information does not represent the actual capabilities of the data cable, for the simple reason that E-Markers can be simulated.

Long-press **`OK`** on this screen to copy the current E-Marker information. The copied E-Marker is saved in "copied emark". The K2 can only save one copied E-Marker at a time. If you want the K2 to carry multiple E-Markers, see [6.4 How to export and import E-Markers](#how-to-export-and-import-e-markers).

### 6.4 How to export and import E-Markers

E-Markers copied by the K2 can be exported to a computer.

Download the [Witrn Firmware Upgrade Software MeterUP v2.6](https://www.witrn.com/witrn/PC/WITRN_USBMeterUP_V26.rar) from the [official website](https://www.witrn.com/?p=2339). After unpacking run `MeterUP.exe`. This application only supports Windows; if the software prompts that .NET is missing, either accept to download it or use the pre-packaged version from the Witrn web page.

![MeterUp1](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/MeterUp1.png)

Click "1 Virtual EMark Settings"; a new screen opens.

![io_E-Marker](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/io_E-Marker.png)

Put the K2 into DFU mode[^6]. Click ② to read the E-Marker previously copied by the K2.

If you need to write E-Markers to the K2, click ③ to select the saved E-Marker parameters. To write multiple parameters, add them multiple times. Click ④ to overwrite the E-Marker list in the K2. The E-Markers previously saved in the K2 will be overwritten.

If you want to customize E-Marker information, you can edit the E-Marker information on the left or import an existing E-Marker for modification. After modification, click "Save Parameters" to save it as E-Marker parameters.

<div style="page-break-before: always;"></div>

## 7 Firmware

### Table of contents

- [7.1 How to enter DFU mode](#how-to-enter-dfu-mode)
- [7.2 How to upgrade the firmware](#how-to-upgrade-the-firmware)

### 7.1 How to enter DFU mode[^6]

As shown in the picture, connect one end of the data cable to the computer. While pressing and holding the **`-`** button on the K2, insert the other end of the data cable into the HID port to enter DFU mode. The other ports cannot flash the firmware. Make sure that you are using a USB-C to USB-C cable; USB-A to USB-C cables will not work. It is also very likely that flashing will only work on real hardware and not on a virtualized Windows operating system.

![DFU](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/DFU.png)

### 7.2 How to upgrade the firmware

Download both the [Witrn USB meter upgrade software](https://www.witrn.com/witrn/PC/WITRN_USBMeterUP_V26.rar) and the [most recent firmware](https://www.witrn.com/?p=2105) from the [official website](https://www.witrn.com/?p=2339). After unzipping the archives, run `MeterUP.exe`. This application only supports Windows; if the software prompts that .NET is missing, either accept to download it or use the pre-packaged version from the Witrn web page.

![MeterUp2](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures-en/MeterUP.png)

Put the K2 into DFU mode. The software will print a message ③ whether the K2 has been detected and is ready for updating. Click ① to select the firmware to upgrade (or downgrade), click ② to write the firmware to the K2, and wait for the progress bar to complete. This indicates that the update is finished. After it has been verified that the firmware was written successfully the K2 will automatically reboot.

<div style="page-break-before: always;"></div>

## 8 Host computer

### Table of contents

- [8.1 Connecting a host computer](#connecting-a-host-computer)

### 8.1 Connecting a host computer

Download the [Witrn Host Computer Curve Software](https://www.witrn.com/witrn/PC/Meter_soft_V3.1.rar) from the [official website](https://www.witrn.com/?p=873). After unzipping, run `WITRN.exe` (only supports Windows systems; if the software prompts that the .NET Core runtime library is missing, install the runtime library either from the internet or by using the archive which is provided for download on the same web page; the x86 version is compatible with x64).

The host computer can be used for data analysis by connecting the computer and K2 via a data cable on the HID port. The software is quite powerful, please refer to the [official instructions](https://www.witrn.com/?p=873) for reference.

<div style="page-break-before: always;"></div>

## 9 Cable resistance

### Table of contents

- [9.1 How to measure cable resistance](#how-to-measure-cable-resistance)

### 9.1 How to measure cable resistance

You need to purchase a cable resistance kit to measure the internal resistance of a data cable. It can be purchased at the Weijian Taobao store.

![GL001](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/GL001.png)

Powered by HID, access it via the Fourth screen -> **Tools** -> **Resistance**.

Connect the components as shown in the diagram below to measure the internal resistance of the data cable.

![htmwr2](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/htmwr2.png)

**Warning:** The resistor will become very hot during measurement. Do not touch it. After measuring the cable resistance, please disconnect the load immediately!

![wire_resistance2](https://raw.githubusercontent.com/ipftalabua/WITRN-K2-Quick-Reference-Manual/refs/heads/main/pictures/wire_resistance2.png)

**Reference Specification:**

Indicates the cable resistance reference data for the reference length.

+ G: Excellent
+ A: Acceptable
+ M: Average
+ P: Discard

The reference specification provides data for four lengths: 0.3m, 1m, 1.5m, and 2m.

**Reference Current:**

Indicates the current that the cable in use can currently handle. It is not the specified maximum it can carry and is for reference only.

**Notes:**
> Both USB-A and C1 ports can be powered by 5V.
>
> C2: Connects to a USB tester with a USB-C port.
>
> A2: Connects to a USB tester with a USB-A port.
>
> GL001 isolation board C2/A2 isolates communication and provides power only.

[^1]: For example, like this.

[^2]: Refers to the method of transmitting real-time data from K2 to a computer. See [8.1 Connecting a host computer](#connecting-a-host-computer)

[^3]: Power Delivery Objects, used to expose the power capabilities of the source port or the power requirements of the receiver.

[^4]: Request Data Objects, used by the receiver port for contract negotiation.

[^5]: "Pass-through" can be understood in the sense of a voltmeter, i.e. the K2 does not interfere with other devices.

[^6]: Device Firmware Upgrade mode, also called firmware flashing mode. See [7.1 How to enter DFU mode](#how-to-enter-dfu-mode)

[^7]: See [6.1 What is/What Does E-Marker Do](#61-What is E-Marker and What Does it Do)

[^8]: See [4.10 What is "PD speedup"](#what-is-pd-speedup)

[^9]: Refers to the other end of the cable not being connected to anything.
