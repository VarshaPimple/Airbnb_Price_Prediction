# Airbnb_Price_Prediction
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import matplotlib.image as mpimg
%matplotlib inline
import seaborn as sns
import warnings
warnings.filterwarnings('ignore')
from datetime import datetime
from scipy.stats import norm


calendar_df = pd.read_csv("calendar.csv")
listings_df = pd.read_csv("listings1.csv")
hosts_df = pd.read_csv("hosts.csv")
reviews_df = pd.read_csv("reviews.csv")

total_rows_cal = calendar_df.shape[0]

#Count total number of unique Listing IDs in the calendar dataset
unique_listing_ids_cal = calendar_df['listing_id'].nunique()

f"Total number of rows in calendar table are {total_rows_cal} and Total Unique listing_ids are {unique_listing_ids_cal}."
Total number of rows in calendar table are 319192 and Total Unique listing_ids are 1749.
