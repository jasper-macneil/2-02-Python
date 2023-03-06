# 2-02-Python# 2-01-Unit-Python
import time 
import board
import digitalio

led = digitalio.DigitalInOut(board.LED)
led.direction = digitalio.Direction.OUTPUT

while True:
    led.value = True
    time.sleep(blinktime)
    led.value = False
    time.sleep(0.5)
    
    blinktime = blinktime + 1000
