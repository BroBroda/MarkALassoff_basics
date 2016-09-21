//: Playground - noun: a place where people can play

import UIKit

//Wywoływanie funkcji_18 september 2016

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
