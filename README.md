# Your Librarian "Amigo"
### Domain
We want to study here authors writing in Spanish from the XX century using data science methods. The analysis of texts from different authors is expected to provide:  
1. Identify the author of a given text by use of supervised learning. Once finished this can be used for author identification of texts with unknown author.
2. Cluster texts from different authors in order to identify similarities between texts and, hence, writing styles.  
3. Within the previously identified clusters carry out sentiment analysis as characterization of the writing styles.

### Data
Only books with public domain will be considered. The texts will be scraped from the following websites:    
..* [www.guttenberg.org](http://www.gutenberg.org/browse/languages/es).  
..* [www.ataun.net](http://www.ataun.net/BIBLIOTECAGRATUITA/indice.html).  
..* [www.dedominiopublico.org](http://www.dedominiopublico.org/libros-2/).  
Text files are available for the books at www.guttenberg.org while mostly pdf files can be obtained for the other two. The conversion from pdf to txt will be carried out using [PDFminer](https://github.com/pdfminer/pdfminer.six).
Once the txt files are collected the books will be divided in chunks to increase the number of available data points.

### Known unknowns  
The available amount of data is regulated with the included number of books and the size of the text chunks for a given book. This issue could be problematic for authors with few available books.  
It is in principle expected that for task 2 different texts for a given author will cluster together but this can not be taken for granted and has to be checked.  
It is unclear if a given cluster could be separated from the other with sentiment analysis (Task 3).
