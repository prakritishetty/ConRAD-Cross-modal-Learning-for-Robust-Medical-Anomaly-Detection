# ConRAD: Cross-modal Learning for Robust Medical Anomaly Detection

## **Project Overview**
 
 Anomaly detection plays a crucial role across various
 fields, especially in domains requiring fine-grained visual
 distinctions, such as industrial quality control and med
ical imaging. Adapting vision-language models (VLMs)
 like CLIP[11] to the medical domain, however, presents
 unique challenges due to the high variability and subtlety
 of anomalies, alongside a scarcity of labeled anomalous ex
amples for training. This study examines leveraging CLIP’s
 zero-shot capability for its direct applicability to medi
cal anomaly detection with minimal architectural modifi
cations. We propose ConRAD, a modified architecture with
 cross-modal vision-language prompt enhancements for im
proving detection in medical contexts. Our findings provide
 insights into the limitations and possibilities for advanc
ing anomaly detection through VLMs, particularly in com
plex, domain-adapted tasks where traditional supervised
 approaches may falter.
 
---

## **Dataset**
BMAD datasets of BrainMRI and Histopathology 

---

## **Results**
![image](https://github.com/user-attachments/assets/ec6651aa-62bd-4297-858b-22ead482f735)

---

## **Conclusion**

Baselines: Compiling our inferences from each of the tasks
 we explored using our baselines the following preliminary
 conclusions were achieved:
 
 • Vanilla CLIP is not adapted well to identifying the nu
ances associated with the images from the medical do
main, and corresponding does not yield very good results
 for medical image anomaly detection.
 
 • A simple two-layer finetuning methodology works better
 for in-domain zero shot detection, but the performance
 drastically degrades in OOD setups. In such a scenario,
 there is a proven need for a more involved associated be
tween image and text features for CLIP to learn better
 representations and hence aid in our task of robust medi
cal image anomaly detection.


 Final Conclusion. Anomaly detection in medical images is
 a challenging task because of the subtle and fine-grained na
ture of medical anomalies. To this end, using VLMs for this
 task explores the usage of text as well as image modalities to
 handle the complexity and variability of annotated medical
 images. Prompt learning is a particularly efficient technique
 that helps fine-tune VLMs for specific downstream tasks
 without the overhead of manual prompt engineering. Yet,
 most prompt-learning approaches only focus on a unidirec
tional prompt-learning pathway, where the textual path is
 oblivious to visual nuances. 
 Our approach bridges this gap
 by introducing two main contributions. The first is learn
able text prompts, which capture the nuances in the visual
 input to the model. The second is the deep prompting to
 the visual encoder by layer-wise projections of the static as
 well as learnable text prompts.
