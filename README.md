# Αλγόριθμοι και πολυπλοκότητα

Γκόγκος Χρήστος @ Τμήμα Πληροφορικής και Τηλεπικοινωνιών, Άρτα, Πανεπιστήμιο Ιωαννίνων

Τελευταία ενημέρωση: 10/12/2021

**~~Πρόοδος στις 9/12/2021~~**

[<mark>Θέματα προετοιμασίας</mark>](./resources/20211202-midterm-prepare.pdf)

**Παρουσιάσεις από το βιβλίο "Αλγόριθμοι Σχεδίαση και Εφαρμογές" των M. Goodrich και R. Tamassia**

* [Κεφάλαιο 1](./resources/ada_book/ch01_gr.pdf)
* [Κεφάλαιο 5Α](./resources/ada_book/ch05/PriorityQueues_gr.pdf)
* [Κεφάλαιο 5Β](./resources/ada_book/ch05/Heap_gr.pdf)
* [Κεφάλαιο 6Α](./resources/ada_book/ch06/Maps_gr.pdf)
* [Κεφάλαιο 6Β](./resources/ada_book/ch06/HashTables_gr.pdf)
* [Κεφάλαιο 6Γ](./resources/ada_book/ch06/CuckooHashing_gr.pdf)
* [Κεφάλαιο 7](./resources/ada_book/ch07_gr.pdf)
* [Κεφάλαιο 8Α](./resources/ada_book/ch08/MergeSort_gr.pdf)
* [Κεφάλαιο 8Β](./resources/ada_book/ch08/QuickSort_gr.pdf)
* [Κεφάλαιο 8Γ](./resources/ada_book/ch08/SortingLowerBound_gr.pdf)
* [Κεφάλαιο 10](./resources/ada_book/ch10_gr.pdf)
* [Κεφάλαιο 11](./resources/ada_book/ch11_gr.pdf)

## Εργασίες μαθήματος ακαδημαϊκού έτους 2021-2022

* [1η εργασία - MAXSUBARRAY](./assignments/2021-2022-prj1/2021f_project1.pdf)
  * [Λύση](./assignments/2021-2022-prj1-sol/README.md)
* [2η εργασία - ΛΑΒΥΡΙΝΘΟΣ (ξένα σύνολα, αναζήτηση κατά πλάτος)](./assignments/2021-2022-prj2/2021f_project2.pdf)
* 3η εργασία

<!-- ## 1. Ανάλυση αλγορίθμων -->


## 5. Ουρές προτεραιότητας και σωροί

* [Οπτικοποίηση](https://www.cs.usfca.edu/~galles/visualization/Heap.html) δημιουργίας σωρού ελαχίστων (MINHEAP) με διαδοχικές εισαγωγές τιμών: π.χ. χρησιμοποιήστε το πλήκτρο **Insert** για τη διαδοχική εισαγωγή των τιμών 21,5,17,12,3,9,16 σε έναν σωρό ελαχίστων
* [Οπτικοποίηση](https://www.cs.usfca.edu/~galles/visualization/Heap.html) δημιουργίας σωρού ελαχίστων (MINHEAP) με τη διαδικασία heapify: χρησιμοποιήστε το πλήκτρο **BuildHeap** για τη δημιουργία ενός σωρού ελαχίστων από έναν πίνακα 31 τιμών με τους ακέραιους από 1 μέχρι και 31
* [Οπτικοποίηση](http://btv.melezinek.cz/binary-heap.html) λειτουργιών insert, delete, heapsort, buildheap σε σωρό μεγίστων (MAXHEAP) 

**Ουρές προτεραιότητας στην Python**

[heapq](https://docs.python.org/3/library/heapq.html)

Παράδειγμα: [heapq_example.py](./heapq_example.py)

**Ουρές προτεραιότητας στην C++**

[std::priority_queue](https://en.cppreference.com/w/cpp/container/priority_queue)

Παράδειγμα: [priority_queue_example.cpp](./priority_queue_example.cpp)

**Ουρές προτεραιότητας στην Java**

[PriorityQueue\<E\>](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/PriorityQueue.html)

Παραδείγματα: [Java PriorityQueue by Programiz](https://www.programiz.com/java-programming/priorityqueue)

**Ασκήσεις**
  
1. Έστω ένας μηχανισμός παραγωγής πραγματικών τιμών. Όταν παράγεται μια νέα τιμή να υπολογίζεται και να εμφανίζεται η διάμεσος από όλες τις τιμές που έχουν παραχθεί μέχρι εκείνη τη χρονική στιγμή. Γράψτε πρόγραμμα που να υλοποιεί τη λύση.
   * Σημείωση 1: η διάμεσος μιας λίστας παρατηρήσεων είναι η τιμή της μεσαίας παρατήρησης στη διατεταγμένη σε αύξουσα σειρά λίστας παρατηρήσεων όταν το πλήθος των παρατηρήσεων είναι περιττό, και το ημιάθροισμα των δύο μεσαίων παρατηρήσεων στη διατεταγμένη σε αύξουσα σειρά λίστας παρατηρήσεων όταν όταν το πλήθος των παρατηρήσεων είναι άρτιο. 
   * Σημείωση 2: Προσομοιώστε την παραγωγή πραγματικών τιμών με μια λίστα  τυχαίων πραγματικών τιμών. Θεωρείστε ότι στη χρονική στιγμή 0 παράγεται η τιμή που βρίσκεται στη θέση 0 της λίστας, στη χρονική στιγμή 1 παράγεται η τιμή που βρίσκεται στη θέση 1 της λίστας κ.ο.κ. 

    ```
    Περιγραφή αλγοριθμικής προσέγγισης

    Δημιουργούνται δύο σωροί, ένας σωρός μεγίστων (ΜΑΧHEAP) και ένας σωρός ελαχίστων (MINHEAP). Η ρίζα του MAXHEAP θα πρέπει να είναι μικρότερη από τη ρίζα του MINHEAP. Αν αυτό δεν ισχύει θα πρέπει να μεταφέρεται η ρίζα του ενός από τους δύο σωρούς στον άλλο σωρό έτσι ώστε να επιβληθεί αυτή η συνθήκη. Οι εισαγωγές νέων τιμών θα γίνονται πάντα στον MAXHEAP. Οι δύο σωροί θα πρέπει να έχουν το ίδιο μέγεθος ή ο ένας να είναι κατά 1 μόνο στοιχείο μεγαλύτερος του άλλου και όταν αυτό παραβιάζεται θα μεταφέρεται η ρίζα του μεγαλύτερου σωρού στον μικρότερο σωρό. Η διάμεσος θα είναι είτε η ρίζα του μεγαλύτερου σωρού είτε το ημιάθροισμα των ριζών των δύο σωρών.

    # Ψευδοκώδικας 
    1. Λήψη νέου ακεραίου και προσθήκη στον MAXHEAP
    2. Αν η ρίζα του MAXHEAP είναι μεγαλύτερη από τη ρίζα του MINHEAP τότε αφαίρεσε τη ρίζα του MAXHEAP και πρόσθεσέ την στον MINHEAP
    3. Αν το μέγεθος των 2 σωρών διαφέρει κατά 2 αφαίρεσε τη ρίζα από το μεγαλύτερο σωρό και πρόσθεσε την στο μικρότερο σωρό.
    4. Η διάμεσος θα είναι o μέσος όρος των κορυφών των 2 σωρών, αν οι σωροί έχουν το ίδιο μέγεθος ή η ρίζα του μεγαλύτερου από τους 2 σωρούς.
    5. Επιστροφή στο βήμα 1 ή τερματισμός
    ```

    * Λύση: [heap_exercise2.py](./heap_exercise2.py)

## 6. Χάρτες    

Οι χάρτες (maps), ή χάρτες κατακερματισμού (hashmaps) ή λεξικά (dictionaries) ή συσχετιστικοί πίνακες (associative arrays) ή συσχετιστικές μνήμες (associative memories) είναι σύνολα ζευγών κλειδί/τιμή. Υποστηρίζουν τις λειτουργίες εντοπισμού (με δεδομένο το κλειδί), εισαγωγής του ζεύγους κλειδί/τιμή΄και διαγραφής (με δεδομένο το κλειδί) με υψηλή ταχύτητα, Ο(1) υπό προϋποθέσεις.

**Λεξικά στην Python**

* [dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
* [υλοποίηση των dictionaries στην Python](https://stackoverflow.com/questions/327311/how-are-pythons-built-in-dictionaries-implemented)
* [The python corner - Python Hash Tables: Understanding dictionaries ](https://thepythoncorner.com/posts/2020-08-21-hash-tables-understanding-dictionaries/)


**Μη διατεταγμένοι χάρτες στην C++**

* [unordered_map](https://en.cppreference.com/w/cpp/container/unordered_map)

Παράδειγμα: [unordered_map_example.cpp](./unordered_map_example.cpp)

**Χάρτες κατακερματισμού στην Java**

* [HashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/HashMap.html)
* [Hash tables in Java](https://www.andreinc.net/2021/11/08/a-tale-of-java-hash-tables)


### Συναρτήσεις κατακερματισμού

**Κρυπτογραφικές συναρτήσεις κατακερματισμού**

* [SHA256 Hash by Blockchain Demo](https://andersbrownworth.com/blockchain/hash)
* [SlavaSoft HashCalc](https://www.slavasoft.com/hashcalc/)

**Παραδείγματα με hash functions στην Python**

* [interactive_py_hash.py](./interactive_py_hash.py)
* [interactive_py_hash2.py](./interactive_py_hash2.py) κρυπτογραφικες συναρτήσεις κατακερματισμού με το module hashlib

**Μη κρυπτογραφικές συναρτήσεις κατακερματισμού (χρήση σε δομές δεδομένων)**

* [General Purpose Hash Function Algorithms](http://www.partow.net/programming/hashfunctions/index.html#AvailableHashFunctions)
* [djb2, sdbm](http://www.cse.yorku.ca/~oz/hash.html)
* [FNV](http://www.isthe.com/chongo/tech/comp/fnv/)
* [murmur](https://www.sderosiaux.com/articles/2017/08/26/the-murmur3-hash-function--hashtables-bloom-filters-hyperloglog/)

**Ελάχιστη τέλεια συνάρτηση κατακερματισμού (minimal perfect hash function)**

Τέλεια συνάρτηση κατακερματισμού είναι μια συνάρτηση κατακερματισμού η οποία αντιστοιχίζει τα στοιχεία ενός συνόλου σε ένα σύνολο ακεραίων χωρίς συγκρούσεις. Ελάχιστη τέλεια συνάρτηση κατακερματισμού είναι μια τέλεια συνάρτηση κατακερματισμού που αντιστοιχίζει χωρίς συγκρούσεις $n$ κλειδιά σε $n$ διαδοχικούς ακεραίους από το $0$ έως το $n-1$.

Δείτε και το [http://cmph.sourceforge.net/concepts.html](http://cmph.sourceforge.net/concepts.html)

### Ανοικτή διευθυνσιοδότηση (open addressing) 

Η ανοικτή διευνσιοδότηση λαμβάνει το όνομά της από την ιδιότητα που έχει να επιτρέπει στα κλειδιά να μετακινηθούν και σε άλλες θέσεις διαφορετικές από τη θέση στην οποία γίνονται αρχικά hash. 

Η ανοικτή διευνσιοδότηση είναι γνωστή και ως κλειστός κατακερματισμός (closed hashing) καθώς τα κλειδία τοποθετούνται μόνο εντός του πίνακα κατακερματισμού και δεν χρησιμοποιείται κάποια άλλη βοηθητική δομή. 

* [Οπτικοποίηση](https://www.cs.usfca.edu/~galles/visualization/ClosedHash.html) ανοικτής διευθυνσιοδότησης

**Παραλλαγές ανοικτής διευθυνσιοδότησης**

* Γραμμική ανίχνευση (linear probing)
* Τετραγωνική ανίχνευση (quadratic probing)
* Διπλός κατακερματισμός (double hashing)
* Τυχαίος κατακερματισμός (random hashing)

### Κλειστή διευθυνσιοδότηση (closed addressing)

Η κλειστή διευθυνσιοδότηση λαμβάνει το όνομά της από την ιδιότητα που έχει να τοποθετεί τα κλειδιά στη θέση στην οποία γίνονται hash, χρησιμοποιώντας μια βοηθητική δομή (π.χ. συνδεδεμένη λίστα) για να αποθηκεύσει στην ίδια θέση πιθανώς περισσότερα από ένα στοιχεία τα οποία γίνονται hash στην ίδια θέση. 

Η κλειστή διευθυνσιοδότηση είναι γνωστή και ως ανοικτός κατακερματισμός (open hashing) και ως ξεχωριστή αλυσίδωση (separate chaining). Το όνομα ανοικτός κατακερματισμός προκύπτει καθώς τα κλειδιά δεν είναι απαραίτητο να βρίσκονται εντός του ίδιου του πίνακα κατακερματισμού, αλλά μπορούν να βρίσκονται σε κάποια βοηθητική δομή.

* [Οπτικοποίηση](https://www.cs.usfca.edu/~galles/visualization/OpenHash.html) κλειστής διευθυνσιοδότησης

### Κατακερματισμός κούκου

Ο κατακερματισμός κούκου πετυχαίνει Ο(1) χρόνο χειρότερης περίπτωσης για αναζήτηση και διαγραφή και Ο(1) αναμενόμενο χρόνο για εισαγωγή.

* [Οπτικοποίηση](https://www.lkozma.net/cuckoo_hashing_visualization/) κατακερματισμού κούκου.


**Ασκήσεις**

1. Γράψτε ένα πρόγραμμα που να δέχεται έναν πίνακα ακεραίων και μια τιμή sum και να εμφανίζει όλα τα ζεύγη τιμών του πίνακα με άθροισμα ίσο με την τιμή sum.
    * Λύση: [hash_exercise1.py](./hash_exercise1.py)
2. Γράψτε ένα πρόγραμμα που να εντοπίζει σε ένα λεξικό με μεγάλο πλήθος λέξεων όλες τις λέξεις για τις οποίες υπάρχουν τουλάχιστον άλλες 4 λέξεις που είναι αναγραμματισμοί της (π.χ. user -> ['rues', 'ruse', 'suer', 'sure', 'user']).
    * Λύση: [hash_exercise2.py](./hash_exercise2.py)
3. Γράψτε ένα προγραμμα που να εντοπίζει το πλήθος των διακριτών ακεραίων σε μια μεγάλη λίστα ακεραίων.
   * Λύση: [hash_exercise3.py](./hash_exercise3.py)
4. Γράψτε ένα πρόγραμμα που να δέχεται έναν πίνακα διακριτών ακεραίων τιμών και να εμφανίζει τον αριθμό κατάταξης κάθε τιμής του πίνακα (π.χ. για τον πίνακα [17, 13, 21, 19] να επιστρέφει [2, 1, 4, 3])
    * Λύση: [hash_exercise4.py](./hash_exercise4.py)
5. Γράψτε ένα πρόγραμμα που να υπολογίζει το πλήθος εμφανίσεων των ελληνικών γραμμάτων (Α-Ω, χωρίς διάκριση σε κεφαλαία ή μικρά) σε ένα δεδομένο κείμενο.
   * Λύση: [hash_exercise5.py](./hash_exercise5.py) 


## 7. Δομές Ένωσης-Εύρεσης (disjoint sets)

* [Οπτικοποίηση δομής ένωσης-εύρεσης](https://www.cs.usfca.edu/~galles/visualization/DisjointSets.html) 

**Ασκήσεις**

1. Δίνεται ένα σύνολο από σχέσεις φιλίας ανάμεσα σε άτομα (κάθε άτομο αναπαρίσταται από έναν αριθμό και η σχέση φιλίας με ένα ζεύγος αριθμών). Εντοπίστε τις ομάδες ατόμων που είναι συνδεδεμένες (π.χ. friends = [[ 1, 0 ], [ 2, 3 ], [ 1, 2 ], [ 4, 5 ]]). 

## 8. Αλγόριθμοι Merge-Sort και Quick-Sort

**Κάτω όριο για ταξινόμηση βασισμένη σε συγκρίσεις στοιχείων**

[Lower bound: Ω(n log n)](https://www.enjoyalgorithms.com/blog/lower-bound-of-comparison-sorting)


## 10. Άπληστοι Αλγόριθμοι

Οι άπληστοι αλγόριθμοι εφαρμόζονται σε προβλήματα που έχουν:
   * την ιδιότητα της **άπληστης επιλογής (greedy choice property)**, δηλαδή μια βέλτιστη λύση να μπορεί να επιτευχθεί επιλέγοντας τοπικά βέλτιστα.
   * την ιδιότητα της **βέλτιστης υποδομής (optimal substructure property)**, δηλαδή η βέλτιστη λύση να μπορεί να σχηματιστεί με βάση βέλτιστες λύσεις σε  υποπροβλήματα του προβλήματος.

Παραδείγματα προβλημάτων που λύνονται βέλτιστα με την άπληστη μέθοδο: κλασματικό πρόβλημα σακιδίου (fractional knapsack), χρονοπρογραμματισμός εργασιών με καθορισμένες στιγμές έναρξης και τερματισμού σε πανομοιότυπες μηχανές, κωδικοποίηση Huffmann.

## 11. Διαίρει και βασίλευε

Αλγόριθμοι διαίρει και βασίλευε: δυαδική αναζήτηση, Merge-Sort, Quick-Sort, πολλαπλασιασμός ακεραίων Karatsuba, πολλαπλασιασμός πινάκων Strassen, μέγιστα σύνολα.

## Aσκήσεις

1. Δίνεται μια ακολουθία μεγάλου μεγέθους με τυχαίες ακέραιες τιμές. Ζητείται να βρεθούν οι 10 πλέον συχνές τιμές χρησιμοποιώντας μια ουρά προτεραιότητας. Αναζητήστε την αποδοτικότερη λύση. Γράψτε πρόγραμμα που να υλοποιεί τη λύση.
   
* Λύση Α: [heap_exercise1a.py](./heap_exercise1a.py)
* Λύση Β: [heap_exercise1b.py](./heap_exercise1b.py)

2. Γράψτε πρόγραμμα που να δέχεται τον αριθμό μητρώου και το όνομα, για 10 φοιτητές. Στη συνέχεια να δέχεται επαναληπτικά αριθμούς μητρώου. Αν ο αριθμός μητρώου δεν υπάρχει στους 10 φοιτητές, το πρόγραμμα να τερματίζει, αλλιώς να εμφανίζει το μήνυμα «Γειά σου » ακολουθούμενο από το όνομα του φοιτητή. Να χρησιμοποιηθεί λεξικό (πίνακας κατακερματισμού).

* [Λύση](./midterm2021_q2.py)

3. Γράψτε πρόγραμμα που με είσοδο ένα μη ταξινομημένο πίνακα A χωρίς διπλότυπα και μια τιμή d, να εκτυπώνει όλα τα ζεύγη τιμών του Α με διαφορά τιμής d. Για παράδειγμα για Α=[1, 5, 6, 2, 7, 4] και d=3 να εκτυπώνει τα ζεύγη (1,4), (2,5), (4,7). Παρατηρείστε ότι τα ζεύγη εμφανίζονται με πρώτο το μικρότερο στοιχείο κάθε φορά.

* [Λύση](./midterm2021_q1a.py)
* [Ταχύτερη λύση](./midterm2021_q1b.py)

<!-- 2. Γράψτε ένα πρόγραμμα που να ανιχνεύει αν σε ένα μη κατευθυνόμενο γράφο υπάρχει κύκλος.  -->


