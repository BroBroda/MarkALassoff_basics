# MarkALassoff_basics
Basics of Swift language created by Mark A Lassoff

//: Playground - noun: a place where people can play

import UIKit

//UIKIt jest odpowiedzilane za połączenie z systemem iOS
//import Cocoa - to biblioteka OS X

var apples = 0
var recipe = 20

if apples > 0
{
    recipe = recipe + 1
    print("Pozostały pewne jabłka.")
}
else
{
    recipe = recipe - 3
    print("Kto zeżarł moje jabłka?!")
}

//apples = -3
print(recipe)
//apples = 6
//print(recipe)


var testScore = 99

if testScore >= 100
{
print("Mamy to! Świetny mecz")
}
else
{
print("Sędzia kaaalosz")
}

var gpa = 3.0
if gpa < 3.0
{print("Otrzymałeś oceną słabsza od dobrej")}
else
{print("Otrzymałeś ocenę co najmniej dobrą")}



//MoreComplexConditionals_27 August (złożone konstrukcje warunkowe ziom)

var citizen: Bool = true
var age:Int = 17

if citizen == true && age >= 18
{
    print("Możesz głosować Panie Dorosły")
} else
{
    print("Nie możesz głosować.Poeszdł mi stąd")
}

var średniaOcen = 3.25
var wynikTestu = 80

if średniaOcen >= 4.0 || wynikTestu >= 80
{
print("Zostałeś przyjęty na studia mądralo")
} else
{
print("Uczelnia nie jest dla ciebie")
}

//EvenMoreComplex? (skomplikowane konstrukcje warunkowe)

/* testScore = 81

if testScore >= 90
{
    print("A")
}
if testScore >= 80
{
    print("B")
}
if testScore >= 70
{
    print("C")
}
if testScore >= 60
{
    print("D")
}  
 //ten kod daje dwie odpowiedzi w przypadku gdy spełniane są 2 warunki: testScore = 72 ---> oceny: C D
 */

testScore = 75
 
 if testScore >= 90
 {
 print("A")
 }
 else  if testScore >= 80
 {
 print("B")
 }
 else if testScore >= 70
 {
 print("C")
 }
 else if testScore >= 60
 {
 print("D")
 } else
{
print("F")
}
/* jesli pierwszy warunek jest prawdziwy zostaje wykoany kawałek kodu (A), reszta zostaje pominięta
Gdy pierwsze polecenie zwraca wartość false zostaje sprawdzone kolejne,
 jesli drugie polecenie jest true - wykonujemy kod, jeśli false - sprawdzamy kolejne polecenie */

//Switch

var grade = "b"
switch grade
{
case "A" , "a":
    
    print("Dobrze. Utrzymuj wynik")
    
case "B" , "b":
    
    print("Kasia dostała piątkę, a Ty nie możesz?")
    
case "C" , "c":
    
    print("Stać Cię na lepszy wynik młoda damo")
    
case "D" , "d":
    
    print("I co z tego że inni też mają dwóję?!")
    
case "F" , "f":
    
    print("Ktoś tu nie będzie miał wakacji..")

default:
    
    print("Jesteś pozaskalowo beznadziejny. Nie ma takiej oceny")
}

//Pętla while: LICZNIK:

var counter = 0
while counter < 21
{
    print(counter)
    counter += 1
}
// idziemy od 0 do 21


//Wykorzystujemy elementy tablicy i ich indeks:

var testScores = [85, 70, 92, 100]
var i = 0
while i < 4
{
    print(testScores[i]) //wyświetl element tablicy pod indeksem [i]
    i+=1
}

//Licznik od 100 do 0 (co 5):

var x: Int = 100
while x > -1
{
    print(x)
    x = x - 5
}


//Pętla FOR

for var i = 0 ; i<21; i += 1
{
    print(i)
}
//odliczniae od 0 do 21

//Petla for i tablica:

var zakupy = ["jajka", "mleko", "płatki", "maka", "sól", "cukier" ]

for var y = 0 ; y<6 ; y++
{
    print(zakupy[y])
}
//Pętla FOR-IN:

var shopList = ["Buddha", "jeans", "sun glasses", "pizza", "new roller skates", "chocolate"]

print("I want:")
for item in shopList
{
    print(item)
}
// item - stała, której przypisana zostaje wartość elementu tablicy

//Pętla for-in przy iteracji przez tablicę zakresu liczb:

for num in 1...6
{
print(num * 5)  //wielokrotności liczby 5
}
