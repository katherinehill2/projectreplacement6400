#!/usr/bin/env python
# coding: utf-8

# In[1]:


import pandas as pd
from bs4 import BeautifulSoup
import requests


# In[2]:


url = "https://www.ncaa.com/rankings/softball/d1/ncaa-womens-softball-rpi"
page = requests.get(url)
soup = BeautifulSoup(page.content, 'html.parser')


# In[13]:


table = soup.find_all('table')
rpi = pd.read_html(str(table))[0]
rpi


# In[12]:


rpi.to_csv(r'C:\Users\Katie\Desktop\softball_rpi_rankings.csv')


# In[ ]:




