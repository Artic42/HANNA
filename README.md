# HANA
Home automation system to control lights, TVs, etc.

## IR Emulator

Small IR transceiver capable of reading an ir remote signal, and store it so it can be send whenever we want. This will allow the system to execute any action controlled by an IR-remote, e.g. Shutdown TV, Raise-Lower volume...

The system will only pass through the command the commands will be stored on the central HANNA HUB, in a database.

### Transceiver

Composed by a raspberry pi Zero W and an Arduino. 3 models exist with different amount of emitters.

Model | Emitters | Receivers
-- | -- | --
HANNA-IR-TR-01 | 1 | 1
HANNA-IR-TR-02 | 2 | 1
HANNA-IR-TR-04 | 4 | 1
HANNA-IR-EM-01 | 1 | 0
HANNA-IR-EM-04 | 4 | 0

### HUB

A SQL database will store the information of each command and each transceiver in the system

## Lights

System to control Wi-Fi lights from TP-Link.

