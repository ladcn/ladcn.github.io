# ladcn.github.io

## Road Status Definition

###### Table 1 Road speed threshold table
| Road grade   | Congestion speed threshold| Unblocked speed threshold |
|:-------------|:--------------------------|:--------------------------|
| 1            | 30                        | 50                        |
| 2            | 20                        | 40                        |
| 3            | 12                        | 25                        |
| 4            | 10                        | 20                        |

Road status categories are based on road grades and road speeds. We classify roads into different grades according to road width, speed limit level, etc. The higher the road grade, the worse the road facility. As shown in Table 1, we use different road speed thresholds to classify road status for different road grades. If the road speed is below congestion speed threshold, the road status is congestion. If the road speed is above unblocked speed threshold, the road status is unblocked. If the road speed is between two threshold, the road status is slow. 

## Evaluation results compared with the historical mode road status.

###### Table 2 Performance comparison
| Methods   | Macro F1 | Unblocked status F1 | Slow status F1 | Congestion status F1 |
|:-------------|:--------------------------|:--------------------------|:--------------------------|:--------------------------|
| HistMode            | 0.3570                        | 0.9197                    | 0.060| 0.091|
| Xgboost            | 0.9047                        | 0.9913                       |0.8110|0.9127|
| GAT            | 0.9053                        | 0.9901                        |0.8082|0.9175|
| L-ADCN            | **0.9105**                        | 0.9911                        |**0.8189**|**0.9216**|

We can observe that HistMode performs significantly worse than any other method in any metrics.
