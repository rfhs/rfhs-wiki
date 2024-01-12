# Wi-Fi Provisioning King of the Hill

An ESP32 will act as an IoT device that needs to be connected to a network to perform it's function.
In the un-provisioned state it provides an interface via BLE to configure the Wi-Fi settings of the target network.
Once connected to the configured Wi-Fi network the ESP32 will make an HTTP GET request to: `hill.rfhackers.com/king.txt`
The HTTP response must be a 200 and the body shall contain your team name.
Upon success, failure, or timeout, the ESP32 will disconnect and revert to it's un-provisioned state.

You must:
- Host a Wi-Fi network for the ESP32 to connect to
- Scan for BLE devices matching: `RFHS_XXXX`
- Calculate CRC32("RFHS_XXXX") for Proof of Possession key 
	- Hint: `CRC32("RFHS_1234") = 0xA84590D6` the proof of possession would be "a84590d6"
- [Provision](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/provisioning/wifi_provisioning.html) the ESP32 via BLE with the settings for their Wi-Fi network
- Successfully respond to the HTTP request made by the client in the allotted time
- Lather, rinse, repeat

