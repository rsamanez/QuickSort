# QuickSort 1'000,000 elements
Assembler x64 Program to sort a random array with 1'000,000 elements

## Algorithm
```
partition(l,h)
 {
   pivot= A[l]
   i=l
   j=h
   while(i<j)
   {
       do
       {
         i++
       }while(A[i]<=pivot)
       do
       {
         j--
       }while(A[j]>pivot)
       if(i<j)
           swap(A[i],A[j])
   }
   swap(A[l],A[j])
   return j
 }
```
## Execution
```
Compile with:
     nasm -f elf64 -o sortRandomArray64.o sortRandomArray64.asm
Link with:
     ld -m elf_x86_64 -o sortRandomArray64 sortRandomArray64.o
Run with:
     ./sortRandomArray64
```
