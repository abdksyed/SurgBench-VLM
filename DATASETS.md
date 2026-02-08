
## Surgical VQA

### EndoVis18-VQA
- Training: 1560 frames with 9014 QA pairs
- Test: 447 frames with 2769 QA pairs
- Template based questions with one word answers
- Eg: What is the state of bipolar forceps?

### Cholec80-VQA
- Training - 21600 frames
- Dataset filter: at least half of the tool tip is visible for tool to be "present" in the frame. Can cause model visual confusion

### SSG-VQA Dataset
- 960,000 QA pairs
- Covers object attributes, spatial relationships, and geometric grounding
- Dataset generated using YOLOv7 detection and DeepLabV3+ segmentation models.

### Surg-396K
- Conversation dataset
- 41400 images
- 396000 conversations in multi-turn format
- pixel level grounding annotations

### SurgVLM-DB
- 23 datasets across 10 distinct surgical tasks
- Standardization of taxonomy
- 1.81 Million Frames
- 7.79 Million QA pairs
- 16 Surgical Types

## Surgical VQLA (Grounded Question Answering)

### Endovis17-VQLA and EndoVis18-VQLA

#### EnvdoVis18
- Training: 1560 frames with 9014 QA pairs
- Test: 447 frames with 2769 QA pairs
- Bounding box for answer of each question or union of tool-tissue.
#### EnvdoVis17
- Primarliy for zero shot eval
- 97 frames with 472 QA pairs manually annotated.

### RIS-VQA
- Source: MICCAI 2017 Robotic Instrument Segmentation Challenge
- Binary VQA with spatial mask
- Example: Is there a [instrument] in this region? ("this region" is defined by a binary mask provided as input)
- or the model maybe asked to predict the region mask.

### INSEGCAT-VQA
- Cataract surgery
- 29380 QA pairs

### Eye PCR
- Grounded in medical knowledge graph
- 25000 triplets 
- Three level: perception, comprehension, and reasoning
- 210000 VQA

## Temporal Surgical VQA

### PSI-AVA-VQA
- From PSI-AVA (Phase, Step, Instrument - Atomic Visual Action) dataset
- Phases (high level stages), Steps (specific goal with a phase), Atomic ACtions (low level movements)
- ~10000 QA pairs with causal and predictive questions
- Example: "What phase follows this one?", "What tool is required for the next step?"

### PitVQA
- Trans-sphenoidal Pituitary Surgery (neurosurgery)
- 25 videos
- 109173 frames, 884242 QA pairs
- integration with surgeon's post operation notes
- Example: "Was a cerebrospinal fluid (CSF) leak observed?"