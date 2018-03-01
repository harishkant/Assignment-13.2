# Assignment-13.2



def fib(n: Int): Int

object patterns {

    def fib(n : Int): Int = {
        @annotation.tailrec
        def go(n: Int, prev2: Int, prev: Int): Int =
            if(n<=0) prev2 
            else go(n-1, prev, prev2+prev)
        go(n, 0, 1)
      }
}
