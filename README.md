# TareaClasesSemana12

```kotlin
/**
 * You can edit, run, and share this code.
 * play.kotlinlang.org
 */
fun main() {
    println("TDD")
    if(sumaParesTest())
    	println("Correcto")
    else
    	println("Error")
        
    if(sumaInparesPrimerTest())
    	println("Correcto")
    else
    	println("Error")
        
    if(sumaInparesSegundoTest())
    	println("Correcto")
    else
    	println("Error")
        
    if(sumaInparesTerceroTest())
    	println("Correcto")
    else
    	println("Error")
        
    if(sumarCuandolosNumerosSonNegativosTest())
    	println("Correcto")
    else
    	println("Error")
}

fun sumaPares(a: Int, b: Int): Int {
    if (a % 2 != 0 || b % 2 != 0 || a <= 0 || b <= 0) {
       return -1
    }
    return a + b
}

// Prueba que Falle
fun sumaParesTest(): Boolean {
    val resp = sumaPares(2, 2)
    val esp = 4
    return resp == esp
}

fun sumaInparesPrimerTest(): Boolean {
    val resp = sumaPares(5, 2)
    val esp = -1
    return resp == esp
}

fun sumaInparesSegundoTest(): Boolean {
    val resp = sumaPares(5, 2)
    val esp = -1
    return resp == esp
}

fun sumaInparesTerceroTest(): Boolean {
    val resp = sumaPares(2, 7)
    val esp = -1
    return resp == esp
}

fun sumarCuandolosNumerosSonNegativosTest(): Boolean {
    val resp = sumaPares(-2, 4)
    val esp = -1
    return resp == esp
}
