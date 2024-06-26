```kotlin
fun main() {
    println("TDD")
    if(validarEdadTest1())
        println("Correcto")
    else
        println("Error")
        
    if(validarEdadTest2())
        println("Correcto")
    else
        println("Error")
        
    if(validarEdadTest3())
        println("Correcto")
    else
        println("Error")
        
    if(validarEdadTest4())
        println("Correcto")
    else
        println("Error")
}

fun validarEdad(edad: Int): String {
    if (edad >= 18 && edad >= 0) {
       return "ACCEPTED"
    } 
    return "REJECTED"
}

fun validarEdadTest1(): Boolean {
    val resp = validarEdad(20)
    val esp = "ACCEPTED"
    return resp == esp
}

fun validarEdadTest2(): Boolean {
    val resp = validarEdad(18)
    val esp = "ACCEPTED"
    return resp == esp
}

fun validarEdadTest3(): Boolean {
    val resp = validarEdad(25)
    val esp = "ACCEPTED"
    return resp == esp
}

fun validarEdadTest4(): Boolean {
    val resp = validarEdad(18)
    val esp = "ACCEPTED"
    return resp == esp
}
