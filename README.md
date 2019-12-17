# Crowd Labeling For Continuous Valued Annotations

The code in this repository is a reimplementation of the work described in **"Modeling annotator behaviors for crowd labeling" [1]** and **"Actively estimating crowd annotation consensus" [2]**.
The original code for the former work was implemented in MATLAB and the latter, a more comprehensive one, was implemented in C++. However, the C++ code is part of a larger project that I am unable to share.

I reimplemented the main part of the code in Python 3.7.3 for reaching a wider range of researchers from various disciplines. The code is unevitably slower than the original C++ implementation. It currently runs on a single core; parallelizing the parameter and consensus update codes should decrease the inference time. Note that the precision of the results may slightly vary due to implementation and hardware differences.

You are encouraged to play around with the code and apply it to your own data for continuous-valued consensus estimation in crowd labeling.

If you use this work, please do not forget to cite the related papers given below. In addition to the papers below [1,2], the detailed descriptions of the models and their derivations can be found in my PhD thesis [3].

 &ndash; Yunus Emre Kara (yekara@yekara.com)
 
 http://yekara.com
## References
1. Kara, Y. E.; Genc, G.; Aran, O.; & Akarun, L. (2015). "[_Modeling annotator behaviors for crowd labeling_](http://yekara.com/pub/kara2015cl.pdf)", Neurocomputing, 160, 141-156.
1. Kara, Y. E.; Genc, G.; Aran, O.; & Akarun, L. (2018). "[_Actively Estimating Crowd Annotation Consensus_](https://doi.org/10.1613/jair.5727)", Journal of Artificial Intelligence Research, 61, 363-405.
1. Kara, Y. E. (2018). "[_Crowd Labeling For Continuous Valued Annotations_](http://yekara.com/pub/kara2018phdthesis.pdf)", PhD Thesis, Bogazici University, Istanbul, Turkey.

## Datasets
- **Age Annotations Dataset**: http://yekara.com/age_annotations/
- **Head Pose Annotations Dataset**: http://yekara.com/headpose_annotations/
