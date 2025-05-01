# Data Card: Labelled Faces in the Wild (LFW)

## Authorship

- **Authors:** Gary B. Huang, Manu Ramesh, Tamara Berg, Erik Learned-Miller  
- **Affiliation:** University of Massachusetts, Amherst  
- **Contact:** [LFW Website]([http://vis-www.cs.umass.edu/lfw/](https://www.aiaaic.org/aiaaic-repository/ai-algorithmic-and-automation-incidents/labeled-faces-in-the-wild-lfw-dataset))  
- **Roles:** Data collection, annotation, publication

---

## Dataset Summary

The LFW dataset contains over 13,000 labeled face photographs collected from the web. Each image is labeled with the name of the person pictured. The dataset is designed for studying unconstrained face recognition.

- **Benefits:** Standard benchmark for face verification and recognition.
- **Known issues:** Images are web-scraped and may contain labeling errors or duplicates.
- **Note:** *The dataset may not be fully representative of global demographics.*

---

## Data Structure

- **Data type:** JPEG images
- **Labels:** Person’s name (string)
- **Features:** Image pixels, file name, label
- **Note:** *No explicit metadata on age, gender, or ethnicity is provided.*

---

## Sensitive Attributes

- **Human-related attributes:** Faces, names
- **Sensitive attributes:** Gender, race, age (not explicitly labeled, but visually present)
- **Discussion:** The dataset may reflect demographic biases present in web images.
- **Note:** *No explicit annotation of sensitive attributes; analysis may require manual inspection.*

---

## Intended Use

- **Intended for:** Face verification, face recognition research
- **Usage guidelines:** For non-commercial research only
- **Train/test splits:** Standard splits provided (View 1 for development, View 2 for testing)
- **Preprocessing:** Images are aligned and cropped; original images also available
- **Note:** *Users should be aware of potential privacy and bias concerns.*

---

## Collection Process

- Images collected from the web using search engines
- Labeled by matching names to images
- **Note:** *Details on annotation process and quality control are limited.*

---

## Evaluation

- **Common benchmarks:** Face verification accuracy
- **Standard protocols:** 10-fold cross-validation, unrestricted and restricted settings
- **Note:** *No evaluation on demographic fairness provided.*

---

## Limitations

- Demographic imbalance (e.g., overrepresentation of certain ethnicities or celebrities)
- Potential labeling errors
- No explicit consent from individuals in images
- **Note:** *Dataset may not generalize to non-celebrity or non-Western faces.*

---

## Additional Notes

- Dataset is widely used but should be applied with caution in sensitive or production settings.
- *Further information on annotation guidelines and demographic breakdown would be helpful.*
