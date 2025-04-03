# 🧬 bulk-rnaseq-postharvest-pipeline

This repository contains a **GitHub Actions workflow** for processing **bulk RNA-seq data from postharvest broccoli samples**. The pipeline is designed to:

- ✅ Perform quality control using **FastQC** and summarize with **MultiQC**  
- ✂️ Trim low-quality reads and adapters with **Trimmomatic**  
- 🎯 Align reads to a reference genome using **HISAT2**  
- 🔄 Convert, sort, and index BAM files using **SAMtools**  
- 💻 Submit jobs to the **UF HiPerGator** (SLURM-based HPC system)  

---

## 📂 Workflow File

The workflow is located at:

```
.github/workflows/rnaseq_pipeline.yaml
```

---

## 🚀 How to Use

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/utsabghimire/bulk-rnaseq-postharvest-pipeline.git
cd bulk-rnaseq-postharvest-pipeline
```

---

## 🧪 Pipeline Steps

| Step            | Description                                          |
|-----------------|------------------------------------------------------|
| **1. QC**        | FastQC & MultiQC for raw read quality assessment     |
| **2. Trimming**  | Trimmomatic removes adapters & low-quality bases     |
| **3. Alignment** | HISAT2 aligns reads to the reference genome          |
| **4. BAM Processing** | SAMtools converts, sorts & indexes BAM files  |
| **5. Job Submission** | SLURM job submitted to UF HiPerGator         |

---

## 🧠 Notes

- The pipeline is intended for **HPC environments** like UF HiPerGator.  
- Ensure that necessary tools (`FastQC`, `Trimmomatic`, `HISAT2`, `SAMtools`) are available on your cluster environment.  
- Modify the workflow YAML and SLURM script templates to match your cluster setup.

---

## 👨‍💻 Author

**Utsab Ghimire**  
*Research Focus: Postharvest Transcriptomics & RNA-seq Pipelines*

---
