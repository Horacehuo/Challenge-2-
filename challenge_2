# import package
import pandas as pd
import numpy as np

def sort_data(data):
    # remove NA values
    clean_data=data.dropna()
    # change Date into one format
    clean_data['Date'] = pd.to_datetime(clean_data['Date'])
    #sort the data as reqiured
    final_data=clean_data.sort_values(by=['Device_ID',"Date"])
    return final_data

#import data to dataframe called data
data=pd.read_csv("random_data.csv")

# run the sort function
final_data=sort_data(data)

# export to into a csv file
final_data.to_csv("random_data_sorted.csv")
