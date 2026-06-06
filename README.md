import time
import datetime
import winsound

set_time = int(input("Enter the duration in minutes: "))
end_time = datetime.datetime.now() + datetime.timedelta(minutes=set_time)

while datetime.datetime.now() < end_time:
    time.sleep(10)  
print("End period!")
winsound.Beep(1500, 3000) 
