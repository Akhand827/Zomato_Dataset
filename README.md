# Zomato_Dataset
1) Learnt about encoding errors.
2) Learnt about matplotlib  figure sizing use rcParams
3) Learnt about why hue did not work in Seaborn as intended.
4) Learnt to understand the difference between value_counts and groupby().size
5) Loved to see how reset_index was being used time and again.


We use hue when we wish to differentiate the categories. But remember the colours of the bar graph were already in different colours. Why was that? In Seaborn library, the default palette is to show a mix of colours for each bar, which we subsequently changed to the colours we wanted. So the hue parameter did not do anything additional in this context. But the hue parameter did give us a legend. 


We used groupby().size plenty of times. I was wondering when to use value_counts and when to use groupby().size 
df[condition] returns a series ==> Here we can use value_counts(). We cant use groupby when it is a series.
df[df[condition]] returns a dataframe ==> We can use groupby().size here. 

Also size gives total count of all elements. If used with a groupby, it gives count of all elements for each group, including null values. But if we use value_counts, we get the element-wise total excluding null values.
