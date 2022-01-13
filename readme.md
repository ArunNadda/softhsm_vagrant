# readme

- this repo is to setup softhsm node
- once started, slot details can be queried using below command

```
$ sudo softhsm2-util --show-slots
Available slots:
Slot 2063597501
    Slot info:
        Description:      SoftHSM slot ID 0x7affffbd
        Manufacturer ID:  SoftHSM project
        Hardware version: 2.2
        Firmware version: 2.2
        Token present:    yes
    Token info:
        Manufacturer ID:  SoftHSM project
        Model:            SoftHSM v2
        Hardware version: 2.2
        Firmware version: 2.2
        Serial number:    ba32d5adfaffffbd
        Initialized:      yes
        User PIN init.:   yes
        Label:            hsm_demo
Slot 1
    Slot info:
        Description:      SoftHSM slot ID 0x1
        Manufacturer ID:  SoftHSM project
        Hardware version: 2.2
        Firmware version: 2.2
        Token present:    yes
    Token info:
        Manufacturer ID:  SoftHSM project
        Model:            SoftHSM v2
        Hardware version: 2.2
        Firmware version: 2.2
        Serial number:
        Initialized:      no
        User PIN init.:   no
        Label:
```
