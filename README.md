from datetime import datetime

def special_dates():
    dates = {
        "Hari Pertama Bertemu": "2023-01-01",
        "Hari Ulang Tahun Kamu": "2024-02-14",
        "Hari Jadi Kita": "2024-03-01"
    }

    today = datetime.now().strftime("%Y-%m-%d")
    
    for occasion, date in dates.items():
        if today == date:
            print(f"Selamat! Hari ini adalah {occasion}!")
        else:
            print(f"{occasion}: {date}")

if __name__ == "__main__":
    special_dates(
