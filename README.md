<div>
    <center>
        <img src="https://github.com/user-attachments/assets/bc4db39d-0447-4f08-be24-1c1f6eb5e8d3" alt="1" width="350" height="350" />
    </center>
</div>

This is the Prototype-v1 VIO-SLAM setup which has embedded "Jetson Nano B01", "IMX219-83 Stereo Camera", "IMU (MPU 9250)", and "GPS (UBLOX NEO-M8N)" in a metal case. Also, there is a 5V fan to cool down the Jetson. For wireless communication with the board, we’ve used a "Wi-Fi adaptor (TP-Link, 150 Mbps)" for now.
We have conducted the calibration process for the cameras, along with some initial testing. Soon, I’ll post the simulation and test results of a VIO algorithm running on this setup.

Also, there will be some modifications for the next version. They are listed here:
1.    Using Waveshare AC8265 Wireless NIC Module for Jetson, instead of the Wi-Fi adaptor ("supports 2.4GHz / 5GHz Dual Band WiFi and Bluetooth 4.2" + "speed: 300Mbps / 867Mbps")
2.    Adding a HC-SR05 ultrasonic sensor to the setup
3.    Using a Waveshare 5inch 800x480 HDMI LCD (H) (*)
4.    Making the setup wheeled, so that the perception and localization information can be used to navigate and control the setup in an indoor environment (**)

* We may decide to use this LCD, or we may choose to keep sending the video wirelessly to the laptop.
** For now, this is not our primary focus. We’re just trying to enhance the robustness of the algorithms and the setup. Also, in the near future, we’ll make the setup airborne (using a Quadrotor, which will require a smaller packaging for the setup).

<div><img src="https://github.com/user-attachments/assets/60e83474-e20d-4584-9a21-c54e45453e02" alt="2" width="250" height="350"/> <img src="https://github.com/user-attachments/assets/fffe2eb4-403a-4eb4-ab04-ff91d0500ecc" alt="3" width="350" height="350"/></div>
