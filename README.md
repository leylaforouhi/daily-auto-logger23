import datetime
import os

def log_today():
    now = datetime.datetime.now()
    log_entry = f"Log entry for: {now.strftime('%Y-%m-%d %H:%M:%S')}\n"

    with open("daily_log.txt", "a") as file:
        file.write(log_entry)

    print("Log saved!")

if __name__ == "__main__":
    log_today()
