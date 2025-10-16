amount = int(input("Enter total amount: "))
note = int(input("Enter highest denomination: "))
notes = [100, 50, 20, 10, 5, 2, 1]
start_index = notes.index(note)
for n in notes[start_index:]:
    count = amount // n
    amount = amount % n
    print(f"{n} rupees note: {count}")
