//# MarkALassoff_basics
//Basics of Swift language created by Mark A Lassoff

//: CHAPTER 2__VARS AND CONS__Zmienne

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


