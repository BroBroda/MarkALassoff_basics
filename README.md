//: Playground - noun: a place where people can play

import UIKit

//Zuzanna_30 august 2016_SLA_Lab3

var age = 23

if age > 59
{
print("To nie koniec życia! Chyba")
}
else if age > 49
{
print("To najprawdopodobniej najbardziej satysfakcjonujący okres w Twoim życiu. Ciesz się rodziną i przyjaciółi!")
}
else if age > 39
{
print("Najlepsza pora, aby zacąć myśleć o emeryturze. Zacznij odkładać hajs")
}
else if age > 29
{
print("Rozwijaj karierę, oszczędzaj. Czas na dzieci i nudne życie")
}
else if age > 19
{
print("Ucz się bo nauka to potęgi klucz, czy jakoś tak")
}
else if age > 11
{
print("Nastolatkiem jest sie raz w życiu. Zrób wypasiona osiemnastkę")
}
else
{
print("Jesteś dzieckiem! Baw się dobrze")
}


var age2: Int = 57

switch age2
{
case 60...130:
    print("Nie jesteś stary, po prostu głupi")
case 50...59:
    print("To naprawdopodobniej Twój kryzys wieku średniego! Albo menopauza..")
case 40...49:
    print("Najlepsza pora, aby się rozwieść")
case 30...39:
    print("Rozwijaj karierę. Kierownikiem maca nie zostaje się od czapy")
case 20...29:
    print("Zdobywaj edukację. Ucz się biologi i chemii he he")
case 12...19:
    print("Nastolatkiem jesteś. Gówniarz")
case 1...11 :
    print("Jesteś dzieckiem! Liż szyby i jedz piasek")
default:
    print("Znak niepoprawny")
}

//zadanie 6:
var x = 12
while x < 109
{
    print(x)
    x = x + 12
}

for var y = 12; y < 110; y = y + 12
{
    print(y)
}
//przykład z modulo
var z = 10
var g = z % 3
print(g)

if g == 0
{
    print("z podzielna przez 3")
} else
{
    print("z niepodzielna/3 ")
}


//przykład pętli FOR-IN
for index in 1..<2
{
    print(index)
}

//drukuje tylko 6, nie inkrementuje !!!!!!!!!!!!!!!
for var h = 6 ; h % 3 == 0  ; h+=1
{
    print(h)
}

//zadanie 7___nie dziala :(
var i = 100
while i > 1 && i % 3 == 0
{
print(i)
i -= 1
}

for var fuck = 100; fuck % 3 == 0 ; fuck-=1
{
    print(fuck)
}
// !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

//zadanie 8/9:

var names = ["Marek", "Tomek", "Jarek", "Ela", "Basia", "Krzysiu", "Robert", "Ignacy"]

for Hej in names
{
//print("Siema \(Hej)!")
print("Yo " + Hej + "!")
}
