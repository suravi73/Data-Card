# Data Card: Labelled Faces in the Wild (LFW)

---
## Dataset Summary
---
Labelled Faces in the Wild (LFW) is a benchmark dataset for face verification, containing over 13,000 labeled face photographs collected from the web. Each image is labeled with the name of the person pictured. The dataset is designed for studying unconstrained face recognition and is widely used for evaluating face verification and recognition algorithms. The images are collected from news articles and other web sources, with the motivation to provide a challenging, real-world dataset for academic research. 

- **Benefits:** Standard benchmark for face verification and recognition.
- **Known issues:** Images are web-scraped and may contain labeling errors or duplicates.
- **Note:** *The dataset may not be fully representative of global demographics.*



### Dataset Link

[http://vis-www.cs.umass.edu/lfw/](http://vis-www.cs.umass.edu/lfw/)

### Data Card Author

Suryalaxmi Ravianandan

---
## Authorship
---

**Publishing Organization:**  
- University of Massachusetts, Amherst

**Industry Type:**  
- Academic - Tech

**Contact Details:**  
- Publishing POC: Erik Learned-Miller  
- Affiliation: University of Massachusetts, Amherst  
- Contact: elm@cs.umass.edu  
- Website: [http://vis-www.cs.umass.edu/lfw/](http://vis-www.cs.umass.edu/lfw/)

**Dataset Owners:**  
- UMass Computer Vision Lab

**Authors:**  
- Gary B. Huang, PhD Student, UMass Amherst, 2007  
- Manu Ramesh, Researcher, UMass Amherst, 2007  
- Tamara Berg, Professor, UMass Amherst, 2007  
- Erik Learned-Miller, Professor, UMass Amherst, 2007

**Funding Sources:**  
- University of Massachusetts, Amherst  
- National Science Foundation (NSF)  
Supported in part by the National Science Foundation under grants IIS-0546666 and CNS-0708344.

**Roles:** 
- Data collection
- Annotation
- Publication

---
## Dataset Overview
---

**Data Subjects:**  
- Non-Sensitive Data about people  
- Sensitive Data about people (faces, names)

**Dataset Snapshot:**  

| Category                | Data                |
|-------------------------|---------------------|
| Size of Dataset         | ~180 MB (compressed)|
| Number of Instances     | 13,233 images       |
| Number of Fields        | 2 (image, label)    |
| Labeled Classes         | 5,749 people        |
| Number of Labels        | 5,749               |
| Average Labels/Instance | 1                   |
| Algorithmic Labels      | 0                   |
| Human Labels            | 13,233              |
| Other Characteristics   | JPEG, 250x250 px    |

**Content Description:**  
Each data point is a JPEG image of a face, labeled with the person's name. Images are collected from the web, primarily news articles.
- **Data type:** JPEG images
- **Labels:** Person’s name (string)
- **Features:** Image pixels, file name, label
- **Note:** *No explicit metadata on age, gender, or ethnicity is provided.*


**Descriptive Statistics:**  
Only count is relevant; other statistics not applicable for images/labels.

| Statistic | image  | label  |
|-----------|--------|--------|
| count     | 13,233 | 13,233 |


---
## Sensitive Attributes
---

**Sensitivity Types:**  
- Identifiable Data  
- User Content (faces, names)

**Fields with Sensitive Data:**  
- `label`: Person's name (identifiable)  
- `image`: Face image (identifiable)
- `Gender, race, age`: not explicitly labeled, but visually present

**Security and Privacy Handling:**  
- Images are publicly available and collected from news sources.
- No explicit consent from individuals.
- Users are advised to use the dataset for research only and not for commercial purposes.

**Risk Types:**  
- Direct Risk (re-identification)  
- Indirect Risk (demographic bias)

**Risk Mitigation:**  
- Use for research only, not for commercial or sensitive applications.  
- Researchers should be aware of bias and report limitations.
  

**Note:** *No explicit annotation of sensitive attributes; analysis may require manual inspection.*

---
## Dataset Version and Maintenance
---

- **Maintenance Status:** Limited Maintenance  
- **Current Version:** 1.0  
- **Last Updated:** 2012  
- **Release Date:** 2007  
- **Maintenance Plan:** No further updates planned. Technical issues may be addressed by the maintainers.

---
## Motivations & Intentions
---

**Purpose:**  *Research*

**Domains of Application:**  
- Machine Learning
- Computer Vision
- Face Recognition
- Face Verification

**Motivating Factors:**  
- *To provide a challenging, real-world dataset for evaluating face recognition algorithms under unconstrained conditions.*

**Intended Use:**  

- *Intended for:* Face verification, face recognition research
- *Usage guidelines:* For non-commercial research only
- *Train/test splits:* Standard splits provided (View 1 for development, View 2 for testing)
- *Preprocessing:* Images are aligned and cropped; original images also available
- *Note:* *Users should be aware of potential privacy and bias concerns.*

**Suitable Use Cases:**  
- Academic research in face recognition  
- Benchmarking face verification algorithms  
- Studying unconstrained face recognition

**Unsuitable Use Cases:**  
- Commercial face recognition products  
- Applications requiring explicit consent  
- Sensitive or privacy-critical applications

**Citation Guidelines:**  
- Cite the original LFW paper.

---
## Provenance
---

**Collection Method:** *Scraped or Crawled*

**Source Description:** *Web images of public figures, collected from news articles and other web sources.*

**Collection Cadence:** *Static (data was collected once)*

**Data Processing:** *Images were aligned and cropped using face detection and manual verification.* 

- **Note:** *Details on annotation process and quality control are limited.*
  
---
## Evaluation
---

- **Common benchmarks:** Face verification accuracy
- **Standard protocols:** 10-fold cross-validation, unrestricted and restricted settings
- **Note:** *No evaluation on demographic fairness provided.*

---
## Limitations
---

- Demographic imbalance (e.g., overrepresentation of certain ethnicities or celebrities)
- Potential labeling errors
- No explicit consent from individuals in images
- **Note:** *Dataset may not generalize to non-celebrity or non-Western faces.*

---
## Additional Notes
---

- Dataset is widely used but should be applied with caution in sensitive or production settings.
- *Further information on annotation guidelines and demographic breakdown would be helpful.*
