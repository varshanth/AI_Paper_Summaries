### ICCV19: Dual Attention Matching for Audio-Visual Event Localization by Wu et. al.

* Prereq: 1803.08842: Audio-Visual Event Localization in Unconstrained Videos by Tian et. al.
* Tackles the Cross Modal and Supervised Multi-Modal Localization Tasks on the AVE Dataset

#### Method/Network: Dual Attention Matching

* Takes advantage on the fact that each segment only contains a single event. In this way, localization is done separately and a single event classification is done separately. The synchronized predicted segments are assumed to be of the predicted event.

* For the cross modal localization task, say A2V, to identify the "l" length visual sequence, we take the global audio feature and the N local visual features and calculate p<sub>t</sub><sup>A</sup> for each t in N. The "l" sized window with the maximum sum of the p<sup>V</sup> values corresponds to the localized visual segment. V2A localization is calculated similarly.

![alt text](Images/19_Dual_Attention_Matching_Method.PNG?raw=true "DAM")

#### Results

![alt text](Images/19_Dual_Attention_Matching_Results.PNG?raw=true "DAM")
