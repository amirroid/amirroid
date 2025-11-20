I'm just an object.
An object that successfully consumed all available memory.
``` kotlin
object IWantAllMemory {
    private val junk = mutableListOf<ByteArray>()

    @JvmStatic
    fun main(args: Array<String>) {
        println("absorbing RAM…")
        while (true) {
            junk += ByteArray(1024 * 1024)
        }
    }
}
```
