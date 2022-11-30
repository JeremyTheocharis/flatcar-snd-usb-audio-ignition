# flatcar-snd-usb-audio-ignition

Transpile ignition.yaml
`cat ignition.yaml | docker run --rm -i ghcr.io/flatcar/ct:v0.9.4 > ignition.ign`
Push to git

Download ipxe iso image
`wget http://boot.ipxe.org/ipxe.iso`

Next press Ctrl+B to get to the iPXE prompt and type in the following commands:
```
iPXE> dhcp
iPXE> chain http://${YOUR_BOOT_URL}
```

Ignition: https://bit.ly/3Vm1a9v
