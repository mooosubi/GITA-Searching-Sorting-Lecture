public class Mergesort
{
 private static double[] temp;
 // Sorts a[0], ..., a[size-1] in ascending order
 // using the Mergesort algorithm
 public static void sort(double[] a)
 {
 int n = a.length;
 temp = new double[n];
 recursiveSort(a, 0, n-1);
 }
 // Recursive helper method: sorts a[from], ..., a[to]
 private static void recursiveSort(double[] a, int from, int to)
 {
 if (to - from < 2) // Base case: 1 or 2 elements
 {
 if (to > from && a[to] < a[from])
 {
 // swap a[to] and a[from]
 double aTemp = a[to]; a[to] = a[from]; a[from] = aTemp;
 }
 }
 else // Recursive case
 {
 int middle = (from + to) / 2;
 recursiveSort(a, from, middle);
 recursiveSort(a, middle + 1, to);
 merge(a, from, middle, to);
 }
 }
