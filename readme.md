# ZMK Config for Sofle
This is a quick config key remap for Sofle Zmk.

|![fe42dadb02df898c0cb13808e3faf62](https://github.com/superxc3/zmk_config_sofle/assets/79617315/aa22f713-3a78-4085-93cd-a2e8c42f69b3)|
|:--:|
| One of our Sofle variant: Sofle Hybrid with Low profile thumb cfx keycap + MX alpha keys Geekark BOW |

1. Use [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/) to remap the keys.
2. This is for Sofle with encoders and oled screen. 

## Bluetooth Connection Manual
|![bluetooth](https://github.com/superxc3/zmk_config_sofle/assets/79617315/dd9db3ed-afc0-4a49-bac2-fe3d8bcff494)|
|:--:|
<br>

## Steps

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/e0200ed6-19f7-4741-9c02-93d3358bd9c2" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>1. Fork this to your github, make sure you have created a github account.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/b30733c7-e8d6-43c0-ac1d-5bb9b6e548b3" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>2. Untick this so it allows you to copy niceview and oled branches, then create <code>fork</code>.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/f3318d8b-c97b-4745-90ac-8871618a5d6b" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>3. Click <code>action</code></td>
  </tr>
</table>


<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/dffcef9d-fd64-45be-8480-d1409f552245" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>4. Click the left <code>.github/workflows/build...</code>, and click <code>Run workflow</code> on right. Wait it run for a few minutes until a green tick.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/adc7d76c-da79-4cd3-9354-4bd467e30292" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
<td>5. Go to <a href="https://nickcoutsos.github.io/keymap-editor/"><code>Keymap Editor</code></a>.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/3acddcbf-2675-417f-9d3d-5d32b44c43b5" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>6. Choose <code>Add/remove repo...</code></td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/a5d41e31-006d-457f-a223-6450b1a86712" alt="Your Image Description" width="400"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>6. Sign in to your github account and <code>select repo..</code>, choose <code>zmk_config_sofle</code> and <code>save</code>.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/f0a6727c-9a2d-40fc-816b-5850a3e2b8ee" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>7. Now choose your repo and correct branch, and you can start mapping. PLEASE CHOOSE NICEVIEW if yours are build with niceview. If yours oled, stick to MAIN will do. This is an important step many people missed! Once it is done click <code>save</code>, wait until it finished compiling then click <code>Latest</code>.</td>
  </tr>
</table>

<table>
  <tr>
    <td><img src="https://github.com/superxc3/zmk_config_sofle/assets/79617315/72fd65f7-8441-4f28-a735-ab1a6976902c" alt="Your Image Description" width="600"></td>
  </tr>
  <tr style="background-color:grey;">
    <td>8. Scroll down and go to download <code>Firmware</code>.</td>
  </tr>
</table>


## Flashing uf2 to split
You may refer to the [demo](https://drive.google.com/file/d/1_iiBsk6CXnIYhRzzQHDtAJCxdc7E1w-u/view?usp=sharing) for flashing procedure. Details as follow:
1. Connect left and right splits to your pc (both connect together using type c cable). You also can flash one side each time without using two cables. 
2. Put right into bootloader mode (press the reset button), one window is popped out showing "nicenano" folder. Dont do anything yet, remember this folder as right split. 
3. Now press reset button on your left split, one window will be popped out as previous step.
4. Drag left and right uf2 to respective folders.
5. Do not disconnect right split yet. 
6. Remove left split from type c cable. Proceed to `First time bluetooth connection` to connect your board to pc. If successfully connected, you shall able to type without cable now. 
8. If so, remove the right split from type c cable. Both should be working good now!
9. If you dont have extra usb c cable...You can do left first, then quickly move to right so the right can sync with left.

</br>

## How to charge?
1. Flip your power button on while charging. If you turn it off means nothing is charged.
2. You can charge both sides together with usb c cable, not a problem.
3. You can charge while using it, but we dont encourage to continuously plugging in because battery may degrades.
4. If you would like to do it in wired mode, you can plug in but flip the power button off. So charging doesnt occur and battery doesnt degrade. 

</br>

## Common Issues and Troubleshooting
1. [Mac or Window OS connected but not responding](https://zmk.dev/docs/features/bluetooth#macos-connected-but-not-working), this is working for Bluetooth 5.2 Windows.
2. Master connected and can type, but not slave refer to [Split Keyboard Halves Unable to Pair](https://zmk.dev/docs/troubleshooting#split-keyboard-halves-unable-to-pair).
3. You may compile the reset.uf2 yourself or get it from [setting reset.uf2](https://drive.google.com/file/d/1r3C8MBEVbgs5SK3Hc2CyoOIaiAPLB_zp/view?usp=drive_link).
4. The board is pre-flashed with the [mouse-native.uf2](https://drive.google.com/drive/folders/1EStNUWT_zY0m-xmcMmOKRE_ifORbUOOl). You may always use these to test the board.
5. No key is registering: have you toggled the power button? (if you have one)

</br>

## Light indicator from Supermini MCU
1. Blue light: you are connected to usb c and the board is charging
2. Slight blue light blinking: you are connected to usb c but not connected to battery. Toggle power button to allow charging.
3. Blink red once: when you toggle the power button on
4. Flashing red: no firmware flashed to the mcu yet

## Light indicator from Nicenano v2 MCU
1. Blue light: you are connected to usb c and the board is charging
2. Blue blinking: bootloader mode, no firmware is loaded

</br>

## Further Troubleshooting Trial and Error
1. For supermini: when i connect cable to pc, double press it, call out a nicenano explorer to lemme drop the new uf2. If i dont drop new firmware and un-plug it, then re-plug back, the nicenano folder will still pop out. I cant type anything. << this is normal.
2. For supermini: by referring to above, if i unplug the cable. Flip power button off and on again. My firmware remains. I can type again, but i did not drop in new firmware. When i plug in the usb, no nicenano folder pop out. << this is normal. 


