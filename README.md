# project1-sequence-analysis
## Identifying mutations in NGS Reads

### Title & purpose

This code compares sequencing reads from S. pombe samples with a reference sequence to identify mismatches between them. It investigates whether treatment using a genotoxic agent changes mutation patterns compared to wild type/controls. 

### How to run the program

Open C7147_Project_1_assessment.ipynb in Google Colab and Run all. The data and reference are downloaded with the first code. 

### Inputs and outputs

Input: a reference string with 200 nucleotides and a list of dictionaries containing information from sequencing reads (read_id, sample, group, sequence).

Output: Summary dictionaries for each sample, two tables for both treatment and control groups (sample results & substitutions)

### Code design

Invalid reads are not included in mismatch statistics, however, they are kept. analyse_reads( ) returns the status of every read as “valid” or “invalid”. The summary shows the amount of invalid reads and excludes them from the percentage calculation. 

Helper functions were defined within the main functions.

### Testing

All functions were tested using constructed test datasets with a range of different types of inputs. Normal inputs, edge cases, and invalid inputs were used to test the code.
