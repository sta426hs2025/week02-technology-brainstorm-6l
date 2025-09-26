Technology: MAS-seq (for single-cell isoform sequencing)

Note: MAS-seq method = Multiplexed Arrays Sequencing method

Background situation: 
It is crucial to understand the isoform-level properties of different cells. Until now, single-cell RNA sequencing methods often only captured short reads, which provide only gene-level information. Other long-read technologies were too inaccurate, preventing a reliable identification to cell barcodes or UMIs.
The solution of this problem was the development of MAS-Seq, which allows for a more detailed view of the transcriptome. 

Advantages:
- full-length isoform information
- reliable cell barcode and UMI detection
- genetic variant detection
- no requirement of orthogonal sequencing methods
- cost-effective
- higher throughput and reduced sequencing needs
- 16-fold throughput increase compared to standard single-cell Iso-Seq libraries

How does it work: 
- Input: Single-cell cDNA (15-75ng), Output: Sequencing-ready library
- Each single-cell RNA transcript is tagged with cell barcode & UMI (droplet methods, e.g. 10x Genomics Chromium)
- Individual cDNA molecules are concatenated into longer fragments
- The concatenated cDNA molecules are sequenced with PacBio HiFi (very accurate long reads)
- Computationally, the concatenated molecules are segmented back into the original individual transcript units. Barcodes and UMIs are extracted and analysed (corrected and deduplicated), isoforms are linked to the cell of origin and its unique transcript molecule.
- A gene- and isoform level matrix that is compatible with standard tertiary analysis tools is output.


Sources:
- https://www.pacb.com/wp-content/uploads/Application-note-MAS-Seq-for-single-cell-isoform-sequencing.pdf, 26.09.2025
- ChatGPT, Prompt: "Please explain how MAS-Seq for single-cell isoform sequencing works"

Authors: 
- Natallia Halai, GitHub username: natalliahalai
- Florian Hellwig, GitHub username: Smile4heWorld