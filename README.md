print("======TICKET CINEMA======")

print("AVAILABLE MOVIES")
print("[SM] SPIDER MAN      :300")
print("[A] AVENGERS         :250")
print("[IM] IRON MAN        :200")
print("[F] FROZEN           :300")
print("[M] MINIONS          :200")
print("[PR] POWER RANGER    :250")

name = input("Enter Customer Name: ")
movie = input("Choose Movies code: ").upper()
qty = int(input("Enter Ticket Quantity: "))

if movie == "SM":
    moviee = "Spider Man"
    price = 300
elif movie == "A":
    moviee = "Avengers"
    price = 250
elif movie == "IM":
    moviee = "Iron Man"
    price = 200
elif movie == "F":
    moviee = "Frozen"
    price = 300
elif movie == "M":
    moviee = "Minions"
    price = 200
elif movie == "PR":
    moviee = "Power Ranger"
    price = 250
else:
    print("Invalid Movie Code!")


if qty >= 4:
    dis = 0.12
elif qty <= 3:
    dis = 0.05
elif qty <= 1:
    dis = 0
else:
    print("No Discount!")

total = price * qty
disc = total - dis


print("========== RECIEPT ===========")
print(f"Customer Name  : {name}")
print(f"Movie Name     : {moviee}")
print(f"Ticket Quantity: {qty}")
print(f"Total          : {total}")
print(f"Discount       : {dis}")
print(f"Total Payment  : {disc:.2f}")

print("===== THANK YOU! =====")

