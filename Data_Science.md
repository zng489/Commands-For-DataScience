
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
  
  `12:31
  
  https://pandas.pydata.org/docs/getting_started/comparison/comparison_with_sql.html
  
  
A	B
0	x	a
1	x	c
2	x	c
3	y	b
4	y	b
 
</p>
```
