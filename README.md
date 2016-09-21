//: CHAPTER 4__ARRAY__Tablice

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


