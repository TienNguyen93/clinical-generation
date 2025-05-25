## Clinical Generation from Doctor-Patient conversation

### Problem statement
Writing clinical notes is a crucial task performed by medical professionals during every patient encounter. However, it is often time-consuming and can contribute to physician 
burnout. Studies discover that physicians spend an average of 52 to 102 minutes per day writing clinical notes based on patient encounters. While these notes are essential for understanding patient history and ensuring continuity of care, the documentation workload contributes to fatigue and burnout. One solution has been to employ medical scribes, which may cost up to $112,000 annually depending on the specialty and institution. These limitations underscore the need for automatic note generation systems that can alleviate documentation burdens.

### Dataset
MTS-Dialog dataset, a curated collection of 1,700 short doctor-patient conversations paired with corresponding summaries. The training set includes 1,201 conversation-summary pairs, while the validation set contains 100 such pairs. 

### Methods
* Leverage pre-trained Flan T5 and BART models from HuggingFace
* Convert the dialog-summary (prompt-response) pairs into explicit instructions
* Explore models' performances in **Zero-shot Inference with prompt template**, **One-shot Inference**, **Few-shot Inference**
* Apply Parameter-Efficient Fine-Tuning (PEFT) adapter

### Evaluation metrics
* ROUGE
