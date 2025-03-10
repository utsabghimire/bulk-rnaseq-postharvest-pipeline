# bulk-rnaseq-postharvest-pipeline


This repository contains a **GitHub Actions workflow** for processing **bulk RNA-Seq data** from **postharvest broccoli samples**. The pipeline is designed to:
- Perform **quality control (FastQC & MultiQC)**
- Trim low-quality reads using **Trimmomatic**
- Align reads to the genome using **HISAT2**
- Convert, sort, and index BAM files using **SAMtools**
- Submit jobs to **UF HiPerGator (SLURM-based HPC system)**

## 📂 Workflow File
The workflow is located at:
.github/workflows/rnaseq_pipeline.yaml


## 🚀 How to Use
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/utsabghimire/bulk-rnaseq-postharvest-pipeline.git
cd bulk-rnaseq-postharvest-pipeline

️ Pipeline Steps
Step	Description
1. QC	FastQC & MultiQC for raw reads
2. Trimming	Trimmomatic removes adapters & low-quality bases
3. Alignment	HISAT2 aligns reads to genome
4. BAM Processing	SAMtools converts & indexes BAM files
5. Job Submission	SLURM job submitted to UF HiPerGator

