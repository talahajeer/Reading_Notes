# Pandas 
## Object creation

* Creating a Series by passing a list of values, letting pandas create a default integer index:

    ```In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])

    In [4]: s
    Out[4]: 
    0    1.0
    1    3.0
    2    5.0
    3    NaN
    4    6.0
    5    8.0
    dtype: float64```

* Creating a DataFrame by passing a NumPy array, with a datetime index and labeled columns:

    ```In [5]: dates = pd.date_range("20130101", periods=6)

    In [6]: dates
    Out[6]: 
    DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
                '2013-01-05', '2013-01-06'],
                dtype='datetime64[ns]', freq='D')

    In [7]: df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

    In [8]: df
    Out[8]: 
                    A         B         C         D
    2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
    2013-01-02  1.212112 -0.173215  0.119209 -1.044236
    2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
    2013-01-04  0.721555 -0.706771 -1.039575  0.271860
    2013-01-05 -0.424972  0.567020  0.276232 -1.087401
    2013-01-06 -0.673690  0.113648 -1.478427  0.524988```

## Viewing Data
 
 * Here is how to view the top and bottom rows of the frame:

    ```In [13]: df.head()
    Out[13]: 
                    A         B         C         D
    2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
    2013-01-02  1.212112 -0.173215  0.119209 -1.044236
    2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
    2013-01-04  0.721555 -0.706771 -1.039575  0.271860
    2013-01-05 -0.424972  0.567020  0.276232 -1.087401

    In [14]: df.tail(3)
    Out[14]: 
                    A         B         C         D
    2013-01-04  0.721555 -0.706771 -1.039575  0.271860
    2013-01-05 -0.424972  0.567020  0.276232 -1.087401
    2013-01-06 -0.673690  0.113648 -1.478427  0.524988 ```   

 * Display the index, columns:

    ```In [15]: df.index
    Out[15]: 
    DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
                '2013-01-05', '2013-01-06'],
                dtype='datetime64[ns]', freq='D')

    In [16]: df.columns
    Out[16]: Index(['A', 'B', 'C', 'D'], dtype='object')  ```  


<br>

DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object.