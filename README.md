## Trustzone Demo on Cortex-M

We want to show in our example “Hello World Cortex-M”  how to setup an example project for the Nuvoton M2351 development board which make use of both worlds, secure and normal world.

Check out our Medium Blogpost [here](https://medium.com/magicofc/gas-for-your-secure-iot-fire-a-tutorial-for-crypto-on-a-cortex-m23-%C2%B5c-bfb27017df21) to get more detailed informations.

----
We will show in our demo the following techniques:
1. Use of GPIO (General Purpose I/O) ports in normal word.
2. Generate an AES 128 bit key for decrypt and encrypt a “secret” value.
3. Initialise UART in both world, for reading from stdin and showing some debug informations.

All actions are handled and evaluated through interrupts.


The following things are needed to start developing:
1. [Nuvoton M2351 development board](http://www.nuvoton.com/hq/products/microcontrollers/arm-cortex-m23-mcus/m2351-series/m2351kiaae/?__locale=en)
2. [OpenNuvoton Software package](https://github.com/OpenNuvoton/M2351BSP)
3. [Keils µVision® IDE - Nuvoton edition](http://www2.keil.com/nuvoton/M0-M23)
Follow the instructions described in the [Board Quick Start Guide.pdf](https://github.com/OpenNuvoton/M2351BSP/blob/master/NuMaker-PFM-M2351%20Board%20Quick%20Start%20Guide.pdf)

4. Place the IoT-Crypto-M23-Trustzone-Demo into the folder "OpenNuvoton Software package\SampleCode\TrustZone"
