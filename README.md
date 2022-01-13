# SHIELD
***Smart Tag-based, Human Infection Reporting and Encounter Logging Device*** (**SHIELD**): A Decentralized, Privacy-Preserving, Acceleration-Proximity-based Contact Tracing Prototype using NodeMCU ESP8266 with an embedded Bluetooth Low Energy (BLE) in the context of the COVID-19 pandemic.

SHIELD contains two devices:

1. **Beacon** used by the general public.
2. **Neuron** used by Authorized Health Officials.

# Tag Configuration

| **Description** | **Key** | **Sample Value** | **Note** |
| ------------- | ------------- | ------------- | ------------- |
| Health Status | HS | U0 | System Defined, see *Health Status Table* |
| CIRRUS Version| CV | 1642088234 | UNIX Time Format |
| ID | ID | 1469781E-3FBC-4985-9423-5083E9E6DCBA | GUID Format |
| MAC Address | MA | {31,42,20,a7,56,0a,4f,2d} | MAC Address on CSV Format inside brackets |
| Contact Number | CN | 9971432991 | Philippines Contact Number Format excluding Country Code |
| Sensor Data | SD | {-12,14,16,5,4,7} | Accelerometer Data (Yaw, Pitch, Roll, x, y, z) |
| Creation Time | CT | 1642088234 | UNIX Time Format |
| Expiration Time | ET | 1642089134 | UNIX Time Format |
| Initialization Vector | IV | y$B&E)H@McQfThWmZq4t7w!z%C*F-JaN | 128-bit Format |
| Integrity Key | IK | 3s6v9y$B&E)H@McQfTjWnZr4u7w!z%C* |  128-bit Format |


**Sample Tag:**
k8mDKG8KNu7iZb01bkg4s5lsp5AfPLBDZE3YlP24yQHSrHDbxidVhphrFCn9z+5Uo/NM9Vc4QPzJoc1i0cCsr2jYDLhCHed3UBgzy8piIL7KwufMhEUdMRJ7/aMQXAttKAttwbWzYJG1x6ctmtarvAm7OcjNQ0sFAKtXMVtBI62wVg48Ld4ffIhCKavUZXMCFDleW70ATPkA2nWHheb5r0/RxnePLDmI79mZ1vaYKJz9ORuQ8SARwbZmUqd42QVHhoYfnXhCLaeGc8vas+dLNV8PSooZgu1lcGsdj6Z/0+aD70DnIKOZ8ViALf6c52Jazaj8iddxXQ7PFd+z2+sS2K6OcCWngyiYA10zKGnFZBrvkLDCayoXw5Tev8Kos4CD

# Health Status Table
The Health Status *HS* are indicators to identify the "Health Status" of the user or its identification in the system.

| **Description** | **Health Status Code** |
| ------------- | ------------- |
| Drop Data Command (Database Command) | U0 |
| Healthy | U1 |
| Positive | U2 |
| Suspected | U3 |
| Recovered | U4 |
| Dead | U5 |
| System Flag - General Status | U6 |
| System Flag - Deactivated Account | U7 |
