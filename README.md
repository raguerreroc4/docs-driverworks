# **Welcome to the DriverWorks Software Development Kit!**

![Logo](https://github.com/control4/docs-driverworks/raw/media/images/logo.png)

The DriverWorks Software Development Kit (SDK) provides dealers and partners with the ability to independently develop custom two-way (Serial & Network) drivers to incorporate new devices into the Control4 environment or to customize existing drivers. DriverWorks uses the Lua programming language, which is delivered within the Composer software application and within the Control4 OS. Completed drivers do not require platform or version-specific compiling. The development kit consists of the Lua Development Environment (included within Composer and the OS), several documentation resources as well sample drivers and code example.

If you are new to the SDK you will find [An Introduction to DriverWorks][1] to be useful reading.


**The latest version of the DriverWorks SDK is 3.2.0. Currently, 3.2.0 is in a beta state. While use of the beta version of the SDK is encouraged and feedback welcome, changes will continue to be made to the contents of the SDK until an official release is delivered. Anticipation of these changes should be considered in your development efforts when using this version of the SDK.**


## DriverWorks Documentation

- The 3.2.0 DriverWorks Fundamentals Guide can be found [here][2].

- The 3.2.0 DriverWorks Proxy and Protocol Guide can be found [here][3].

- The 3.2.0 DriverWorks API Reference Guide can be found [here][4].


## DriverWorks Development Resources

The directories at the top of this page contain various resources to support your driver development efforts. They include:

#### Driver Development Templates
The SDK includes numerous Driver Development Templates to help jump start your development efforts. Currently, the following Proxies are supported with a Template:

- AV Switch
- Blind
- Doorstation
- DVD
- Generic Proxy
- IP Camera
- Lock
- Pool
- Projector
- Receiver
- Security Controller
- Thermostat
- TV

#### Icon Templates

The DriverWorks SDK provides templates and instructions on how to create icons that will blend in with the default icons inside Control4 interfaces. Conforming to these guidelines insures that custom icons feel like part of the system. 

#### Media Service Proxy

Control4’s Media Service Proxy (MSP) provides a layer of commands, notifications, events and other data handling elements that will support the development of drivers for media-based services and devices. This iteration of a media-focused proxy represents a new direction in driver development as it uses Control4’s .c4z driver architecture and offers the ability to support XML-based user interfaces.

From an end user perspective, drivers written against the Media Service Proxy will be able to provide a user interface that can browse cloud based media services consistently across numerous navigator devices. The proxy is designed to be platform independent with regard to devices displaying its user interface while maintaining the ability to easily integrate with new clouds or devices introduced to the Control4 system.


#### QR Branding

Composer Express supports the ability for a device driver to be downloaded by way of scanning a Quick Response code (QR code). QR codes are useful as they can be placed on a product, product packaging, within documentation or embedded on a product webpage.  When scanned within the Composer Express (CE) environment, they not only provide a way to download the correct driver, but also offer a convenient way to build a project at an offsite location.


#### Sample Drivers

The DriverWorks SDK provides code examples as well as sample drivers which are useful in understanding some of the more complex areas of device driver development. The examples found here is referred to throughout the SDK documentation. This directory serves a collection area for that code. 

#### Table Logger Utility

The Table Logger utility has been provided to assist driver developers in identifying areas within their driver that may be using a growing amount of memory. The utility is executed from within ComposerPro at the driver level on the Lua tab. The utility code is copied into the driver's Lua Command window. Once executed, the Lua output contains an iterated list of all Lua tables found within the driver at the time of execution. This list of tables can then be reviewed for suspect table entries or tables with anonymously added entries (using table.insert) that may be growing over time without any checks.

[1]:	https://control4.github.io/docs-driverworks-introduction/#introduction
[2]:	https://control4.github.io/docs-driverworks-fundamentals/#introduction
[3]:	https://control4.github.io/docs-driverworks-proxyprotocol/#introduction
[4]:	https://control4.github.io/docs-driverworks-api/#introduction
