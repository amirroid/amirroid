``` kotlin
object Amirroid {
    private val junk = mutableListOf<ByteArray>()

    @JvmStatic
    fun main(args: Array<String>) {
        while (true) {
            junk += ByteArray(1024 * 1024)
        }
    }
}
```
