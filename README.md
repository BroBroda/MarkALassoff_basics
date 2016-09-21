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


func formulaPitagoras(sideA: float_t, sideB: float_t)
{
    var sideC = (sideA * sideA) + (sideB * sideB)
    sideC = sqrt(sideC)
    print(sideC)
}

//formulaPitagoras( 5 , 6)
