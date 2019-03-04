# dataQA

Relation validation dataset - dataQA

This is a relation validation dataset called dataQA. It is composed of 10578 examples, 8728 for training and 1850 for test. It was built by  exploiting the WebQuestion (Berant et al., 2013) in a distant supervision process.  WebQuestion is a well-known dataset of questions and answers pairs.  This dataset adapt well to our setup because the questions were posed without knowing the KB schema and answers are entities from. 

DataQA consists of annotated sentences separated by “\t”. For example the line:

```yaml
1122	wqr001085	/location/location/containedby	Alexandria	Egypt	the main sport that interests alexandrians is football , as is the case in the rest of egypt and africa . alexandria stadium is a multi-purpose stadium in alexandria , egypt .	C	21	17
``` 

It’s a positive example of the relation “/location/location/containedby” between Alexandria and Egypt entities. Both, training and test, partitions were balanced to guarantee equal positive and negative examples.

If you use this dataset, please cite:

```yaml
@inproceedings{moreno2019archsiamoise,
  title={Architecture siamoise et embeddings de triplet pour la validation de relation},
  author={Moreno, Jose G and Rahman, Rashedur  and Rudnik, Charlotte  and Wang, Cong  and Grau, Brigitte},
  booktitle={Conférence en Recherche d'Information et Applications (CORIA2019)},
  year={2019}
  }
``` 
