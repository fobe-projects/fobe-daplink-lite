# FoBE CMSIS-DAP Lite
CMSIS-DAP Firmware.

## Firmware
FoBE CMSIS-DAP Lite based on WCH CH32V203 (support crystal-less USB), supports SWD, JTAG and CDC.

On Properties for DAPLink -> C/C++ Build -> Settings -> C Compiler -> Preprocessor page:
* Define `DAP_FW_V1`: generate CMSIS-DAP V1 firmware, using HID transport protocol.
* Do not define `DAP_FW_V1`: generate CMSIS-DAP V2 firmware, using WINUSB transfer protocol.

### Pin map
|  FUNC    | Pin   |
|  :----   | :---- |
| SWD_CLK  | PA.1  |
| SWD_DIO  | PA.0  |
| SWD_RST  | PA.4  |
| CDC_TXD  | PA.2  |
| CDC_RXD  | PA.3  |
| JTAG_TDI | PA.7  |
| JTAG_TDO | PA.6  |

### Product Document
[FoBE CMSIS-DAP Lite](https://docs.fobestudio.com/product/f2211)