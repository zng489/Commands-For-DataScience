
# Filter out corrupt data


```
##### Print out the number of missing values per column
** df.isnull().sum())
__df.isnull().sum())__

*df.isnull().sum())__
```

```
##### Print out the number of missing values per column
** df.isnull().sum())
__df.isnull().sum())__

*df.isnull().sum())__

```
df.unique()d

```
<p>df.dropna()

  <br>df.dropna()
  
  <br> SELECT * FROM table LIMIT ==> df.head(7)
  
  <br> SELEC name FROM table ==> df[['name']]
  
  <br> SELECT * FROM table WHERE Pclass = 3 ==> df[df['Pclass'] == 3]
  
  <br> SELECT * FROM table WHERE Pclass = 3 and sex = 'male' ==> df[(df['Pclass'] == 3) & (df['Sex'] == 'male')]
  
  <br> SELECT * FROM table WHERE Pclass = 3 OR sex = 'male' ==> df[(df['Pclass'] == 3) & (df['Sex'] == 'male')]
  
  <br> SELECT * FROM table ORDER BY Pclass ==> df.sort_values(by='Pclass', ascending=False)
  
  <br> SELECT Pclass, COUNT (*) FROM table GROUP BY 1 ==> df.groupby('Pclass').count()
  
  <br> SELECT COUNT (*) FROM table ==> df.groupby('Pclass').size()
  
| Tables        | A | B |
| ------------- |:-:|:-:|
| col 3 is      | x |   |
| col 2 is      | ce|   |
| zebra stripes | a |   |
  
  
  
  
    A	B
  0	x	a
  1	x	c
  2	x	c
  3	y	b
  4	y	b

  df.groupby('B').size()
  B
  a    1
  b    2
  c    2
  dtype: int64
  
  
  <br> SELECT COUNT (*) FROM table ==> df[['Pclass', 'PassengerId']].groupby('Pclass').count()
  
  A	B
0	x	a
1	x	c
2	x	c
3	y	b
4	y	b

df[['A', 'B']].groupby('A').count()

  B
A	
x	3
y	2

<br> SELECT Sex, AVG(age), COUNT (*) FROM table GROUPBY 1 ==> df.groupby('C').agg({'B':np.mean, 'A':np.size})

A	B	C
0	x	1	a
1	x	2	c
2	x	3	c
3	y	4	b
4	y	5	b

	B	A
C		
a	1.0	1
b	4.5	2
c	2.5	2

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

  
  `12:31
  
  https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_sql.html
  
  
  
|                      SQL                     |                 Pandas                |
|:--------------------------------------------:|:-------------------------------------:|
| select * from airports                       | airports                              |
| select * from airports limit 3               | airports.head(3)                      |
| select id from airports where ident = 'KLAX' | airports[airports.ident == 'KLAX'].id |
| select distinct type from airport            | airports.type.unique()                |


```

* SELECT, WHERE, DISTINCT, LIMIT
* Here are some SELECT statements. 
* We truncate results with LIMIT, and filter them with WHERE. We use DISTINCT to remove duplicated results.

|                      SQL                     |                 Pandas                |
|:--------------------------------------------:|:-------------------------------------:|
| select * from airports                       | airports                              |
| select * from airports limit 3               | airports.head(3)                      |
| select id from airports where ident = 'KLAX' | airports[airports.ident == 'KLAX'].id |
| select distinct type from airport            | airports.type.unique()                |
