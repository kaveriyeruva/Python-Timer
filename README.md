import time
import datetime
import winsound

set_time = int(input("Enter duration in minutes: "))
end_time = datetime.datetime.now() + datetime.timedelta(minutes=set_time)

print(f"⏳ Timer started for {set_time} minutes...")

while datetime.datetime.now() < end_time:
    time.sleep(10)  # check every 10 seconds

print("End period!")
winsound.Beep(2000, 1000)  # frequency, duration
