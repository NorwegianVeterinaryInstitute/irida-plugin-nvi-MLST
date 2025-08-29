## Main finding
If two schemes have same similarity score (0-100), MLST tool will choose one with smaller ST number
  F. ex: ecoli (ST 25) and ecoli_4 (ST 45) has idential score of 100 against the input sequences, MLST will choose ecoli (ST 25) as the final result. 

# Test data and results from 

| Sample_ID             | Scheme | ST |
|------------------------|--------|----|
| 2025-01-7255-1-1-2-1   | ecoli  | 74 |


### Full results: 

```
$VAR1 = [
          'ecoli',
          74,
          '6/5/4/2/6/7/2/4',
          100
        ];

$VAR2 = [
          'ecoli_4',
          88,
          '6/4/12/1/20/12/7',
          100
        ];
```        
| Sample_ID             | Scheme | ST |
|------------------------|--------|----|
| 2025-01-7364-1-1-2-1  | ecoli  | 2 |


### Full results:
```
$VAR1 = [
          'ecoli',
          2,
          '8/2/7/3/7/1/4/2',
          100
        ];
$VAR2 = [
          'ecoli_4',
          10,
          '10/11/4/8/8/8/2',
          100
        ];
```
| Sample_ID             | Scheme | ST |
|------------------------|--------|----|
| 2025-01-8368-2-1-1-1  | ecoli  | 3 |


### Full results
```
$VAR1 = [
          'ecoli',
          3,
          '3/8/5/11/8/3/5/3',
          100
        ];
$VAR2 = [
          'ecoli_4',
          69,
          '21/35/27/6/5/5/4',
          100
        ];
```
| Sample_ID             | Scheme | ST |
|------------------------|--------|----|
| 2025-04-19620-4-2-1-1  | ecoli_4  | 117 |

```
$VAR1 = [
          'ecoli_4',
          '117',
          '20/45/41/43/5/32/2',
          100
        ];
$VAR2 = [
          'ecoli',
          '-',
          '2/11/23/136/10/15/10/~12',
          86
        ];
```
