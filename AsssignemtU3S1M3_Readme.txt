
root@f15e8fa2ccf5:/# pip3 install lambdata_henry      
Collecting lambdata_henry
  Using cached https://files.pythonhosted.org/packages/2f/bd/1cdd7a5b55e1d7c4b5272a8f551b64df69ca31a44a39b003dce5ec2dbef3/lambdata_henry-0.0.3-py3-none-any.whl
Requirement already satisfied: pandas in /usr/local/lib/python3.7/dist-packages (from lambdata_henry) (1.1.0)
Requirement already satisfied: numpy in /usr/local/lib/python3.7/dist-packages (from lambdata_henry) (1.19.1)
Requirement already satisfied: python-dateutil>=2.7.3 in /usr/local/lib/python3.7/dist-packages (from pandas->lambdata_henry) (2.8.1)
Requirement already satisfied: pytz>=2017.2 in /usr/local/lib/python3.7/dist-packages (from pandas->lambdata_henry) (2020.1)
Requirement already satisfied: six>=1.5 in /usr/lib/python3/dist-packages (from python-dateutil>=2.7.3->pandas->lambdata_henry) (1.12.0)
Installing collected packages: lambdata-henry
Successfully installed lambdata-henry-0.0.3
root@f15e8fa2ccf5:/# python3
Python 3.7.3 (default, Jul 25 2020, 13:03:44) 
[GCC 8.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import pandas as pd
>>> import numpy as np
>>> import lambdata_henry as lh
>>> lh.get_state_from_abbreviation('AK')
'Alaska'
>>> lh.get_abbreviation_from_state('Alaska')
'AK'
>>> lh.date_extract(pd.DataFrame({'date': ['2018-08-09 11:10:55','2019-03-02 13:15:21']}))
                  date  year  month  day
0  2018-08-09 11:10:55  2018      8    9
1  2019-03-02 13:15:21  2019      3    2
>>> 








