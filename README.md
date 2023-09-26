# Countdown-timer
import time
hours = int(input("Enter hours: "))
minutes = int(input("Enter minutes: "))
seconds = int(input("Enter seconds: "))
print(f"Countdown started for {hours:02d}:{minutes:02d}:{seconds:02d}")
total_seconds = hours*3600 + minutes*60 + seconds
while total_seconds > 0:
    print(f"{total_seconds//3600:02d}:{(total_seconds//60)%60:02d}:{total_seconds%60:02d}")
    time.sleep(1)
    total_seconds -= 1
