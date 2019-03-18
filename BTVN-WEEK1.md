# BTVN
homework for android with kotlin class
fun DnaToRna(DNA: String)
{ 
    for (A in DNA) {
  		when (A){
            'G' -> print("C")
            'C' -> print("G")
            'A' -> print("U")
            'T' -> print("A")
        }
    }
}

fun ToAcronym(Name: String)
{
var list = Name.split(" ")
for( x in list)
print(x.take(1))
}

fun BTVN3(Number: Int) { 
    if (((Number % 3) != 0) && ((Number % 5) != 0) && ((Number % 7) != 0))
    {
        print (Number)
        return
    }
	for (i in 3..7 step 2)
    if ((Number % i) == 0)
    when (i){
                3 -> print("Pling")
                5 -> print("Plang")
                7 -> print("Plong")
    }
}
fun main() {
    BTVN3(34)
    println()
    ToAcronym("Nguyen Cuong Liem")
    println()
    DnaToRna("GCTGCAGTACG")
}
