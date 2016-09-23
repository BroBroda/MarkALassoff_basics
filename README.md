//: CHAPTER 5__FUNKCJE__18 september 2016

import UIKit

//Wywoływanie funkcji_18 september 2016

func sayHello()
{
print("Witaj!")
}


sayHello()
sayGoodbye()


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
    var greetingNumber = randomInt(0, max:greetings.count - 1)
    return greetings[greetingNumber]
}
//Wykorzystujemy funkcję randomInt jako indeks funkcji randomGreeeting

print(randomGreeting())
print(randomGreeting())
print(randomGreeting())


//Zasięg zmiennej

var score = 1000
let width = 10.55
print("Zmienna na zewnątrz funkcji: \(score)")
print("Stała na zewnątrz funkcji: \(width)")
print()
func myfunc()
{
    print("Zmienna wewnątrz funkcji: \(score)")
    print("Stała wewnątrz funkcji: \(width)")
    var funcVar = 55
    print("Zmienna funcVar wewnątrz funkcji: \(funcVar)")
}

myfunc()
/*  print("Zmienna funcVar wewnątrz funkcji: \(funcVar)")
    Próba uzyskania dostępu do zmiennej funcVar  na zawnątrz funckji kończy się błędem
    bo jest to zmienna O ZASIĘGU LOKALNYM   */


func twoNumbers(numA: Int, numB: Int)
{
    print("\(numA)  \(numB)")
}
twoNumbers(4, numB: 9)








