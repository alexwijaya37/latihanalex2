import pandas as pd
data = pd.read_csv (r'/Users/user/Desktop/Data_Science/contohdata.csv', delimiter=';',error_bad_lines=False)
print(data)
data1 = pd.DataFrame(data, columns= ['Client Name','Country'])
print(data1)
data2 = pd.DataFrame(data, columns= ['Product', 'Purchase Price'])
print(data2)
data1.to_csv('data_1.csv')
data2.to_csv('data_2.csv')
