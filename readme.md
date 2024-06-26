# Topsis-Ayun-102167007

Topsis-Rohan-Gulati is a Python library designed for addressing Multiple Criteria Decision Making (MCDM) problems using the Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) method.

## Installation

You can install the library using pip:


```bash
pip install Topsis-Rohan-Gulati
``` 

## How to Use

To use the library, provide the CSV filename with the ".csv" extension, the weights vector with comma-separated values, the impacts vector with comma-separated signs (+,-), and the output CSV filename with the ".csv" extension.

Example:
```bash
Topsis sample.csv "1,1,1,2,2" "+,+,-,+,+" result.csv
```

## Input (sample.csv)

Fund Name,P1,P2,P3,P4,P5

M1,0.68,0.46,4,52.7,14.46

M2,0.61,0.37,6.9,51.5,14.85

M3,0.61,0.37,4.4,53.5,14.72

M4,0.7,0.49,6,54.5,15.42

M5,0.65,0.42,4.1,68.7,18.47

M6,0.62,0.38,3.6,36.4,10.25

M7,0.92,0.85,5.2,44.6,12.89

M8,0.81,0.66,3.7,35.9,10.27

## Command

```bash
Topsis sample.csv "1,1,1,2,2" "+,+,-,+,+" result.csv

```

## Output (result.csv)

Fund Name,P1,P2,P3,P4,P5,Topsis Score,Rank

M1,0.68,0.46,4.0,52.7,14.46,0.5903064989592446,4.0

M2,0.61,0.37,6.9,51.5,14.85,0.5408709514358343,5.0

M3,0.61,0.37,4.4,53.5,14.72,0.5933191124418361,3.0

M4,0.7,0.49,6.0,54.5,15.42,0.4714313335411608,7.0

M5,0.65,0.42,4.1,68.7,18.47,0.3803866453639049,8.0

M6,0.62,0.38,3.6,36.4,10.25,0.9855303249104818,1.0

M7,0.92,0.85,5.2,44.6,12.89,0.5209148114910495,6.0

M8,0.81,0.66,3.7,35.9,10.27,0.7535236734320149,2.0

## Other Notes

The library removes the first column and first row from the CSV before processing to eliminate indices and headers. Ensure your CSV follows the format as shown in the sample.csv.
Make sure the CSV does not contain categorical values.

