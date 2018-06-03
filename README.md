# USRP nRF24 demodulator
nRF24LU1+ (and derivatives') packet demodulator GRC (v3.7.11) diagram for Ettus USRP SDRs. Based on [the one for HackRF](https://wiki.bitcraze.io/misc:hacks:hackrf).

Captured packets are pushed into a FIFO under ```/tmp/fifo``` which then can be used with omrilluz's nRF24 decoder (https://github.com/omriiluz/NRF24-BTLE-Decoder) like:

```cat /tmp/fifo | ./nrf24-btle-decoder```

Tested with USRP B200.
