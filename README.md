# BLAST Sequence Analysis

This project uses **NCBI BLAST** (Basic Local Alignment Search Tool) to analyze a given nucleotide sequence and retrieve similar sequences from the NCBI database. The results are parsed from XML and converted into an HTML report.

## Features
- Uses `Bio.Blast.NCBIWWW` to perform BLAST searches.
- Parses BLAST results using `xml.etree.ElementTree`.
- Generates an HTML report listing sequence matches.

## Requirements
Ensure you have Python installed along with the necessary dependencies:

```sh
pip install biopython
```

## How to Use
1. **Clone the Repository**
   ```sh
   git clone https://github.com/hiirrs/IF3211-NCBI-BLAST-Exploration.git
   cd IF3211-NCBI-BLAST-Exploration
   ```
2. **Run the script**
   ```sh
   python main.py
   ```
3. **View Results**
   - The results will be saved in `blast_results.html`. Open it in a web browser to see the BLAST search matches.

## File Structure
```
📂 Project Folder
├── main.py             # Main script for BLAST search
├── README.md           # Documentation
└── blast_results.html  # Generated BLAST result (the existed script is from the existed sequence search)
```

## Example Output
The BLAST search results are saved in `blast_results.html` in the following format:
```html
<html>
  <body>
    <h1>BLAST Results</h1>
    <ul>
      <li>Homo sapiens brain-expressed HHCPA78 homolog VDUP1 (Gene) mRNA, complete cds</li>
      <li>Homo sapiens thioredoxin interacting protein (TXNIP), transcript variant 1, mRNA</li>
      ...
    </ul>
  </body>
</html>
```

## Notes
- Ensure you have an active internet connection while running the script as it queries NCBI databases.
- The sequence used in this script is a **FASTA sequence** of a human gene.

## License
This project is open-source and licensed under the MIT License.
