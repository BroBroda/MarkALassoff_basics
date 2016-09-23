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
print()

func twoNumbers(numA: Int, numB: Int)
{
    print("\(numA) \(numB)")
}
twoNumbers(4, numB: 9)

//print("\(numA)  \(numB)")     - argumenty funkci maja zasięg LOKALNY a nie GLOBALNY ziom




//Funkcje zagnieżdżone = f. zadeklarowana w bloku innej funkcji

func nested(i: Int, j:Int)
{
    func printAnswer(answer:Int)
    {
        print("\(answer)")
    }
    
    var sum = i + j
    printAnswer(sum)
}

nested(5, j: 6)

print()

//Ćwiczenia_23/09/2016_SLA_Lab5

/*
func mojaFunkcja(rows:Int , columns:Int) -> String
{
    let gwiazda = ["osioł"]
    return gwiazda[0]
    print(gwiazda[0])
}
mojaFunkcja(3, columns: 5)
*/


let gwiazdy = ["*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*", "*"]

for k in gwiazdy
{
    print(gwiazdy)
}




let animals = ["kot", "pies", "ryba"]
for zwierzak in animals
{
    print(animals)
}




