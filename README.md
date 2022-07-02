# internet-kill-switch
C programming project to implement serial-radio connection and toggle power relays


The Internet Kill Switch

I am working on a coding project, for fun and to build my understanding of programming in C.  Here are some of the goals I hope to accomplish: 

1. Program two low-cost microcontrollers in C (EFM8 Busy Bee)
2. Use SPI to connect to two radio modules (RFM69)
3. Over the license-free ISM band, instruct a relay to close or open
4. Increase my understanding of the Simplicity Studio environment
5. Implement step debugging methods within Simplicity Studio

This project serves a particular purpose in our house - there are times when the draw of streaming services is too strong (especially around bedtime), and it can be hard to step away.  This device provides discreet recourse for a parent, grandparent, or babysitter.  The user device is a box with a big red button, as well as a green and a red light.  The colored lights show the internet status as up and down, respectively.  The box is battery powered.  

The automation device is installed between the internet router and modem, and their DC power supplies.  This device has two separate relays that can interrupt the power to the modem and router (simultaneously).  The relays would then latch in that state until directed otherwise.  Power to the MCU would be redirected from from one of the power supplies, and through a small buck converter.  

This is a work in progress, and the code will be posted on my GitHub page: 
https://github.com/larrabeelabs/internet-kill-switch
