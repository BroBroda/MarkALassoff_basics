/*

//# MarkALassoff_basics
//Basics of Swift language created by Mark A Lassoff

import Cocoa

var numOfStudents = 10
let pi = 3.1415

numOfStudents = 5
numOfStudents = 7  //przywołuję zmienną, więc nie muszę juz dodawać przedrostka "var"

//pi = 4.15        //stała nie może się zmieniać heh

var age = 40    //niejawne określanie typu zmiennej

var ageOfAnt:Float = 3.464646
var numOfItems:Int = 77        //wyraźne określanie typu zmiennej
//numOfItems = 86.6
var name:String = "Mark Lassoff"
var myName = "Zuzanna Adamczyk"


let anInt: Int = 32
let blabla: Int32 = 1234567890
let blablabla: Int16 = 12345
let bla:Int8 = 123

let aFloat:float_t = 10.005  //t = type
let bFloat:Float = 9.04
let aDouble: double_t = 10.00000005

let aBoolean: Bool = true
let mojeBiurko: String = "Lampa"

let anImplicitInteger = 32

var anImplicitFloat = 10.5

// var newVariable = anInt + aFloat   nie można dodawać Int do Float

let a = 10
var b = 5

var c = a + b
print(c)

var d: Float = 1782 - 695.44
print(d)

var e: Int = 72 * 109
print(e)
var f = 9087 / 16.55
print(f)

var g = 10 % 7
print(g)


b++              //postfiks - działa na zmiennej po przeprowadzeniu obliczeń
print(b)
++b             //prefiks - inkrementuje/dekrementuje wartość przed obliczeniem
print(b)

++c
print(c)


var value = 145
//value = 149.3

var secondValue = 99.92
//secondValue = 85
var secondValue2 = Int(secondValue)
print(secondValue2)


var preciseValue = Double(value)
print(preciseValue)
preciseValue = preciseValue + 0.86512874
print(preciseValue)

var intValue = 3
var floatValue = Double (intValue)
print(floatValue)

var cookies = 5
print("Mamy")
print(cookies)
print("ciastek.")

let firstName = "Zuzanna"
let lastName = "Adamczyk"
print(firstName + lastName)
print(firstName + " " + lastName)

print("Mamy " + String(cookies) + " ciastek")       //Konkatencja ciągów tekstowych
print("Mamy \(cookies) ciastek.")                   //Interpolacja ciągu tekstowego
print("Nazywam się \(firstName) \(lastName)")
print("Mój pies ma \(3*7) psich lat.")


/* SLA_Lab2
 ZuzannaAdmaczyk_26 August
 */

let score: Int = 67
let rate: float_t = 12.5
let gpa:float_t = 4
let name2: String = "Bill Johnson"
let nameGPA: String = "Jane Smith \(gpa)"
let exactValue: double_t = 27.82354

var operand1 = 47.98
var operand2 = 78.881
print((operand1) + (operand2))

*/


import UIKit

var animals: [String] = ["pies", "kot", "koń", "mysz", "aligator", "szczur", "słoń", "żaba", "ślimak"]

var gpas: [Double] = [3.25, 2.54, 1.2, 3.98, 4.0, 2.911, 2.05, 3.91]

let tablicaX : [String] = ["My", "cat", "is", "dead"]

/*
 var i = 0...7
print(animals[i])


 animals[3] = "jastrząb"
 print(animals[3])
 
 
for var j = 0 ; j < 8 ; j+=1
{
print(animals[j])
}
*/

for k in animals
{
 print(k)
}

gpas.count
print(gpas.count)   //drukuj ile jet wartości w tablicy gpas

animals.count
print(animals.count)    //drukuj ile jet wartości w tablicy animals

print("Tablica zwierząt zawiera \(animals.count) wartości")

/*for var x = 0 ; x < gpas.count; x+=1
{
print(gpas[x])
}
*/
print("a nawet szybciej:")

for y in 0..<gpas.count
{ print(gpas[y]) }

print(animals[0...2])

print(gpas[0..<gpas.count])

animals[0...3]





var multiplesOfThree: [String] = []
if multiplesOfThree.isEmpty
{print("Tablica multiplesOfThree jest pusta")}

var multiple = 0

while multiple < 100
{
    multiplesOfThree.append("\(multiple)")
    multiple += 3
}

for var multiple1 = 0; multiple1 < 100; multiple1 += 3
{ print(multiple)}
// wychodzi "102" 34 razy? wtf




var teams: [String] = ["Yankees", "Mets", "Giants", "Liberty", "Red Bulls", "Rangers", "Nets"]

var ingredients: [String] = []

if teams.isEmpty
{print("Tablica teams jest pusta")}
else {print("Tablica teams jest wypełniona")}

if multiplesOfThree.isEmpty
{print("Tablica multiplesOfThree jest pusta")}
else {print("Tablica multiplesOfThree jest wypełniona")}


if ingredients.isEmpty
{print("tak pusto")}


teams.count
teams.append("Devils")
teams.insert( "Barcelonaaa", atIndex:1)
teams.count




ingredients.append("cebula")
print(ingredients.count)
var newIngredients: [String] = ["jajka", "cukier", "masło"]
ingredients += newIngredients
ingredients += ["ciastka", "więcej ciastek" , "jeszcze więcej ciastek"]

ingredients.insert("środek przeczyszczający" , atIndex:0)
print(ingredients)


//ingredients.removeAll()
ingredients.removeFirst()
ingredients.removeLast()
if ingredients.isEmpty == false
{
 ingredients.removeAtIndex(5)
}
print(ingredients)
ingredients.isEmpty

var pustaTablica:[Int] = []
if pustaTablica.isEmpty
{
print("PustaTablica jest pusta")
}

