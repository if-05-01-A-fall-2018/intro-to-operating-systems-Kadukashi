# QNX
## Basic Information
QNX is a commercial real-time operating system that was developed by Canadian company Quantum Software Systems.
The product was originally developed in the early 1980s and ultimately acquired by BlackBerry in 2010.
QNX was one of the first commercially successful microkernel operating systems and is used in a variety of devices including cars and mobile phones.

## Technology insight
The QNX kernel contains only CPU scheduling, interprocess communication, interrupt redirection, and timer.
Everything else is done by a special process called proc.
This performs the process creation and memory management by working in conjunction with the microkernel.
There are no device drivers in the kernel. The network stack is based on NetBSD code.

QNX interprocess communication consists of sending a message from one process to another and waiting for a response.
This operation is called MsgSend.
The message is copied by the kernel from the address space of the send process to that of the receiving process.
When the receiving process waits for the message, control of the CPU is transmitted at the same time without passing through the CPU scheduler.

## Some interesting stuff
1. Apple's CarPlay runs on it. While some may find this unbelievable, Apple has been a long-time partner of QNX.
2. Boeing relies on it for its defense systems even while it develops the competing Black phone (which runs on the notoriously unsecure Android platform)
3. Ford quietly drops Microsoft in favor of QNX as it will be less expensive and address complaints about malfunctioning technology.
