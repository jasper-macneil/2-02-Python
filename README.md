# 2-02-Python# 2-01-Unit-Python
import time 
import board
import digitalio

led = digitalio.DigitalInOut(board.LED)
led.direction = digitalio.Direction.OUTPUT

blink_time = 1

while True:
    print("In loop")
    led.value = True
    time.sleep(blink_time)
    print(blink_time)
    led.value = False
    time.sleep(0.5)
    
    blink_time = blink_time + 1
