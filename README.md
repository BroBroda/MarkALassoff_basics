//: Array & Dictionary_Tablice i Słowniki
import UIKit


var  gpas: [String : Float] = ["Kowalski" : 3.01, "Nowak" : 5.0, "Wiśniewski":2.995, "Lewandowski" : 4.567, "Feret":1.87 , "Majowska":6.0]

print(gpas)

print(gpas["Feret"])

for (name, grade) in gpas
{
    print("\(name): \(grade)")
}

var students = [ 1234: "Adamczyk", 3456: "Nowakowksa", 9876: "Kowalczykówna", 1005: "Zieliński", 2211:"Kamiński"]


students[9785] = "Woźniak"            //dodaliśmy Wożniaka
students[9876] = "Kowal"              //zastępiliśmy Kowalczykównę. A co!
print(students)

var replacedValue = students.updateValue("Jankowski", forKey: 2211)
print("Zastąpiona wartość to \(replacedValue)")

students.updateValue("Adam", forKey: 1234)

for (idNumber, lastName) in students
{
    print("\(idNumber) : \(lastName)")
}

students[1005] = nil //usuwamy Zielińskiego; klucz 1005 nie będzie miał przypisanej wartośći

var deletedValue = students.removeValueForKey(3456)
print("Usunięta wartość to: \(deletedValue)")
print(students.count)


// Zuzanna_14 september 2016_SLA_Lab4

var shoppingList = ["jaja", "mleko", "soda", "masło", "chleb", "jogurt", "ser", "piwo", "kurczak", "jabłka", "gruszki"]

print(shoppingList[4])
print(shoppingList[7])

//shoppingList.insert("wino", atIndex: 7)
shoppingList[7] = "winiacz"

print("Na liście zakupów jest \(shoppingList.count) produktów")



var nowySlownik = ["JFK": "John F. Kannedy International Airport", "LGA" : "LaGuardia Airport", "BDL" : "Bradley International Airport", "FLL":"Ft.Lauderdale International", "LAX":"Los Angeles Airport"]


nowySlownik.updateValue("TF Green Airport", forKey: "PVD")
nowySlownik.updateValue("San Francisco International Airport", forKey: "SFO")

for (skrot, nazwaLotniska) in nowySlownik
{
print("\(skrot) to skrót dla \(nazwaLotniska)")
}

nowySlownik.removeValueForKey("BDL")

