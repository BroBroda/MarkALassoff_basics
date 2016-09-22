//: CHAPTER 5__FUNKCJE__18 september 2016

import UIKit

//Wywoływanie funkcji:

func sayHello()
{
print("Witaj!")
}

sayGoodbye()
sayHello()

func sayGoodbye()
{
    print("Nara!")
}

func sayGreeting(name: String)
{
    print("Zamknij się \(name)")
}

sayGreeting("Tomek")



//a2 + b2 = c2 (kwadrat)
func formulaPitagoras(sideA: float_t, sideB: float_t)
{
    var sideC = (sideA * sideA) + (sideB * sideB)
    sideC = sqrt(sideC)
    print(sideC)
}

//sqrt(sideC) - (sideC) do kwadratu

formulaPitagoras( 12, sideB: 9)
formulaPitagoras(12, sideB: 5)


//5.2 Funkcje zwracające wartość

func randomInt(min: Int, max:Int) ->Int
{
    return min + Int(arc4random_uniform(UInt32(max - min + 1)))
}
/*      return - wynik tego polecenia będzie wartością zwrotną
        arc4random_uniform()- wartość zwrotna to losowa wybrana liczba całkowita (UInt32)
        z zakresu od 0 do wrtości w nawiasie (w argumencie funkcji)
        WYNIK: losowo wybrana liczba z zakresu od min do max        */


print(randomInt(0, max: 10))



func randomGreeting() -> String
{
    var greetings = ["Witaj", "No yo", "Siema", "Dzień doberek", "Sto lat", "Uszanowanko", "Hej", "Cześć", "Hola"]
    greetings.count
    var greetingNumber = randomInt(0, max:8)
    return greetings[greetingNumber]
}

print(randomGreeting())
print(randomGreeting())
print(randomGreeting())


