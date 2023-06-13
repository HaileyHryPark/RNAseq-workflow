RNA-Seq Workflow
================

##### Original Repository Forked from Thomas W. Battaglia (https://github.com/twbattaglia/RNAseq-workflow)

``` bash
# Install git (if needed)
conda install -c anaconda git wget --yes

# Clone this repository with folder structure into the current working folder
git clone https://github.com/HaileyHryPark/RNAseq-workflow.git

# Change directory into the new folder
cd new_workflow
```

##### Folder Structure

``` bash
── new_workflow/
  │   └── annotation/               <- Genome annotation file (.GTF/.GFF)
  │  
  │   └── genome/                   <- Host genome file (.FASTA)
  │  
  │   └── input/                    <- Location of input  RNAseq data
  │  
  │   └── output/                   <- Data generated during processing steps
  │       ├── 1_initial_qc/         
  │       ├── 2_trimmed_output/     
  │       ├── 3_final_qc/           
  │       ├── 4_aligned_sequences/  <- Main alignment files for each sample
  │       ├── 5_final_counts/       <- Summarized gene counts across all samples
  │  
  │   └── star_index/               <-  Folder to store the indexed genome files from STAR 
```
