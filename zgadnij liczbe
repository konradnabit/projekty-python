import random
import time
def gra():
    liczba = random.randint(1, 100)
    imie = input().strip()
    print("\nWpisz imię:")                                                #Gracz wpisuje swoje imie
    print('Jeżeli będziesz chciał/ła przerwać grę, wpisz "koniec".')      #Gra informuje o możliwości przerwania wpisując koniec
    time.sleep(1)
    print(f'Cześć {imie}! Zagrajmy w grę. Wpisz liczbę od 1 do 100.')

    proby = 0                                                              #Licznik prób

    while True:
        wpis = input("Twoja liczba: ")
        if wpis.lower() == "koniec":
            print(f"Koniec gry. Wylosowana liczba to: {liczba}. Do zobaczenia, {imie}!")
            break

        if not wpis.isdigit():
            print("To nie jest liczba! Spróbuj jeszcze raz.")
            continue

        x = int(wpis)

        if x < 1 or x > 100:
            print("Liczba nie mieści się w zakresie 1–100.")
            continue

        proby += 1

        if x > liczba:
            print('Za dużo.')
        elif x < liczba:
            print('Za mało.')
        else:
            print(f'Gratulacje {imie}! Zgadłeś/-aś liczbę w {proby} próbach.')
            break

# 🔁 Główna pętla gry
while True:
    gra()
    ponownie = input("\nCzy chcesz zagrać ponownie? (tak/nie): ").strip().lower()
    if ponownie != "tak":
        print("Dzięki za grę! Do zobaczenia!")
        break
