# Pandas
pandas is a fast, powerful, flexible, and easy to use open-source data analysis and manipulation tool, built on top of the Python programming language..

>> you should import pandas into your project!


### pandas is well suited for many different kinds of data:

* Tabular data with heterogeneously-typed columns, as in an SQL table or Excel spreadsheet

* Ordered and unordered (not necessarily fixed-frequency) time series data.

* Arbitrary matrix data (homogeneously typed or heterogeneous) with row and column labels

* Any other form of observational / statistical data sets. The data actually need not be labeled at all to be placed into a pandas data structure
<br>
<hr>

## The most elementary functions of pandas
1. Reading data : `data = pd.read_csv('my_file.csv')`

2. Writing data : `data.to_csv('my_new_file.csv', index=None)`

3. Checking the data : `data.shape OR data.describe()
Seeing the data : data.head(3) OR data.loc[8] OR data.loc[8, 'column_1'] OR data.loc[range(4,6)]`

<br>

## The basic functions of pandas

### Logical operations :
```
data[data['column_1']=='french']

data[(data['column_1']=='french') & (data['year_born']==1990)]

data[(data['column_1']=='french') & (data['year_born']==1990) & ~(data['city']=='London')]

data[data['column_1'].isin(['french', 'english'])]
```
<br>

### Basic plotting

```
data['column_numerical'].plot()

data['column_numerical'].hist()
%matplotlib inline/
```
<br>

### Updating the data

```
data.loc[8, 'column_1'] = 'english'

data.loc[data['column_1']=='french', 'column_1'] = 'French'
```

### Medium level functions
* Counting occurrences
```
data['column_1'].value_counts()
```

### Operations on full rows, columns, or all data
```
data['column_1'].map(len)

data['column_1'].map(len).map(lambda x: x/100).plot()

data.apply(sum)
```

### Correlation and scatter matrices
```
data.corr()

data.corr().applymap(lambda x: int(x*100)/100)

pd.plotting.scatter_matrix(data, figsize=(12,8))
```
<br>

### Advanced operations in pandas

* The SQL join

```
data.merge(other_data, on=['column_1', 'column_2', 'column_3'])
Grouping

data.groupby('column_1')['column_2'].apply(sum).reset_index()
```

* Iterating over rows

```
dictionary = {}

for i,row in data.iterrows():
dictionary[row['column_1']] = row['column_2']
```

<br>
<br>
<hr>

**Always** you can contact me [Here](https://3madov-77.github.io/Side-Projects/Me/index.html)

<br>
<br>
<br>
<br>

[`Back To The Main Page`](https://3madov-77.github.io/Reading-Notes/)