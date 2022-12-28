# 60key-ortholinear
A 5x12 ortholinear keyboard using a Raspberry Pi Pico

## Bill of Materials
* Case (see below)
* PCB (see below)
* Raspberry Pi Pico (with separate pin headers)
* 60 switches (I used Brown Gateron)
* 60 1N4148 diodes
* 60 1u keycaps

### Case
I have 3D designed a case specifically for this keyboard. It requires 4 M2.5x12mm screws.

### PCB
Gerber files have been uploaded to this repository, and a service such as JLCPCB can be used to order PCBs.

## Assembly
Complete these steps in order:
* Place the pin headers on the back, and apply solder on the front. Cut the excess flush with the PCB.
* Place diodes on the back, and apply solder on the front. Cut the excess flush with the PCB.
* Insert switches to the front of the case, mindful of orientation with the PCB.
* Place the PCB onto the switches, and apply solder on the back.
* Place the Raspberry Pi Pico on the pin headers and apply solder.
* Place the two halves of the case together and secure using screws.
* Place keycaps on switches.

## Code
First, [install CircuitPython](https://learn.adafruit.com/welcome-to-circuitpython/installing-circuitpython). Then, copy `keyboard.py` to the Raspberry Pi Pico.

The layout of the keyboard can be viewed [here](http://www.keyboard-layout-editor.com/##@_name=60key%3B&@=%0A%0A%0A%60%0A%0A%0A%0A%0A%0AEsc&=%0A%0A%0AF1%0A%0A%0A%0A%0A%0A1&=%0A%0A%0AF2%0A%0A%0A%0A%0A%0A2&=%0A%0A%0AF3%0A%0A%0A%0A%0A%0A3&=%0A%0A%0AF4%0A%0A%0A%0A%0A%0A4&=%0A%0A%0AF5%0A%0A%0A%0A%0A%0A5&=%0A%0A%0AF6%0A%0A%0A%0A%0A%0A6&=%0A%0A%0AF7%0A%0A%0A%0A%0A%0A7&=%0A%0A%0AF8%0A%0A%0A%0A%0A%0A8&=%0A%0A%0AF9%0A%0A%0A%0A%0A%0A9&=%0A%0A%0AF10%0A%0A%0A%0A%0A%0A0&=%0A%0A%0AF11%0A%0A%0A%0A%0A%0ABack%3B&@_a:7%3B&=Tab&=Q&=W&=E&=R&=T&=Y&=U&=I&=O&=P&_a:4%3B&=%0A%0A%0AF12%0A%0A%0A%0A%0A%0AEnter%3B&@_a:7%3B&=Del&=A&=S&=D&=F&=G&=H&=J&=K&=L&=%2F%3B&='%3B&@=Shift&=Z&=X&=C&=V&=B&=N&=M&_a:4%3B&=%0A%0A%0A-%0A%0A%0A%0A%0A%0A,&=%0A%0A%0A%2F=%0A%0A%0A%0A%0A%0A.&=%0A%0A%0A%5B%0A%0A%0A%0A%0A%0A%2F%2F&=%0A%0A%0A%5D%0A%0A%0A%0A%0A%0A%5C%3B&@_a:7%3B&=Prt%20Sc&=Ctrl&=Super&=Alt&=Fn%201&=&=&=Fn%202&_a:4%3B&=%0A%0A%0AH%0A%0A%0A%0A%0A%0A%2F&larr%2F%3B&=%0A%0A%0APD%0A%0A%0A%0A%0A%0A%2F&darr%2F%3B&=%0A%0A%0APU%0A%0A%0A%0A%0A%0A%2F&uarr%2F%3B&=%0A%0A%0AE%0A%0A%0A%0A%0A%0A%2F&rarr%2F).
