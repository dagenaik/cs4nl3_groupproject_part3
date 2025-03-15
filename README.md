# cs4nl3_part3
- `Instructions.pdf` contains the instructions for the assignment
- `cleaned_combined.csv` is the cleaned and combined data with columns `tweet,label,annotator_id`. This dataset has 996 instances (after removing tweets with no annotation and some tweets that were annotated multiple times by the same annotator)
  - `tweet` corresponds to a tweet
  - `label` is an integer between 1.0-5.0
  - `annotator_id` is an integer that corresponds to the partition this tweet came from. For example, the person who annotated parition 1 has their data saved as `1.db`, and `annotator_id=1` for all tweets they annotated.
 - `anotation_analysis.ipynb` contains the notebook used to collect, clean and analyze the data
   - krippendorff's alpha was used as an agreement metric since there was some data with missing annotations
   - majority vote was used as a ground truth label as it was the most practical
