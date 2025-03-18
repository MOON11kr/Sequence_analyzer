Sequence Analyzer is a Python package designed to analyze and process sequences such as DNA, RNA, protein, and numerical sequences. It provides powerful functions for sequence statistics, pattern recognition, similarity analysis, and transformation operations.

Installation
Install the package via pip:
pip install sequence-analyzer

 Usage:
You can use sequence_analyzer for various types of sequence analysis. Below are some examples:

1️⃣ Checking if a sequence is valid
python
Copy
Edit
from sequence_analyzer import is_valid_dna

sequence = "ATCGTAGC"
print(is_valid_dna(sequence))  # Output: True


2️⃣ Counting nucleotide occurrences
python
Copy
Edit
from sequence_analyzer import count_nucleotides

sequence = "ATCGATCG"
print(count_nucleotides(sequence))  
# Output: {'A': 2, 'T': 2, 'C': 2, 'G': 2}


3️⃣ Finding GC Content (%)
python
Copy
Edit
from sequence_analyzer import gc_content

sequence = "ATGCGC"
print(gc_content(sequence))  
# Output: 50.0

4️⃣ Reverse Complement of a DNA Sequence
python
Copy
Edit
from sequence_analyzer import reverse_complement

sequence = "ATCG"
print(reverse_complement(sequence))  
# Output: 'CGAT'


5️⃣ Finding a Pattern in a Sequence
python
Copy
Edit
from sequence_analyzer import find_pattern

sequence = "ATCGATCGATCG"
pattern = "TCG"
print(find_pattern(sequence, pattern))  
# Output: [1, 5, 9]


6️⃣ Translating a DNA sequence to Protein
python
Copy
Edit
from sequence_analyzer import translate_dna
sequence = "ATGTTTGGG"
print(translate_dna(sequence))  
# Output: 'MFG'


⚡ Features
✔ Validates DNA, RNA, and protein sequences
✔ Counts nucleotides and amino acids
✔ Calculates GC content
✔ Finds patterns in sequences
✔ Converts DNA to mRNA and proteins
✔ Generates reverse complements
✔ Supports FASTA file reading and writing

📜 Available Functions
Function Name and	Description
is_valid_dna(seq)	Checks if a sequence contains only valid DNA bases (A, T, C, G).
count_nucleotides(seq)	Counts occurrences of nucleotides in a DNA sequence.
gc_content(seq)	Calculates the GC content percentage.
reverse_complement(seq)	Generates the reverse complement of a DNA sequence.
find_pattern(seq, pattern)	Finds all occurrences of a pattern in a sequence.
translate_dna(seq)	Translates a DNA sequence into a protein.
