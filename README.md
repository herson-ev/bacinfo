# bacinfo
Simple python script mapping BACnet element names and their corresponding numeric code.
So far only BACnet objects and properties are included in the script.
The code is *not* meant to be robust. It will crash if you request unavailable elements.
It simply saves me some time on my daily tasks.

It is possible to query BACnet elements either by name or numeric code. Check some examples below.
## BACnet Objects
    $bacinfo -o 23
    accumulator
    $bacinfo -o 2
    analog-value
    $bacinfo -o analog-input
    0
    $bacinfo -o analog-output
    1

## BACnet Properties
    $bacinfo -p 22
    cov-increment
    $bacinfo -p object-name
    77
