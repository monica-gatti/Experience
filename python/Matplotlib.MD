
```
matplotlib.pyplot.hist(x, bins=None, range=None, density=False, weights=None, cumulative=False, bottom=None, histtype=’bar’, align=’mid’, orientation=’vertical’, rwidth=None, log=False, color=None, label=None, stacked=False)
```

Parameter	Description
x:	This denotes the input parameter in the form of arrays.  
bins:	This denotes the range of values. It can accept both integer and sequence values.  
range:	The lower and upper range of bins is included through this parameter.  
density:	This generally contains boolean values and is denoted as density = counts / (sum(counts) * np.diff(bins)).  
weights:	This parameter denotes the weight of each value.  
cumulative:	This parameter denotes the count of each bin together with the count of the bin for previous values.  
bottom	This denotes the location of the baseline of each bin.  
histtype	This parameter is used to denote the type of histogram to be plotted.For example:bar,bar stacked,step or step filled. If you do not mention anything it will take the bar as the default.
align	This will help you in deciding the position of the histogram. For example Left, right or middle. It will take the middle as the default.  
orientation	This parameter helps you to decide whether you want to plot your histogram horizontally or vertically. It will take default as vertical.  
rwidth	This parameter helps you in setting the relative width of the bars with respect to bin width.  
color	This parameter will help you in setting the color of sequences.  
label	This command will help you in setting the labels for your histogram plot.  
stacked	This parameter takes boolean values(True or False). If you pass it as False then data will be arranged in a side-by-side manner if you have given histtype as a bar or else if it is a step, the data will be arranged on top of each other. If you have passed this parameter as True the data will be stacked on top of each other.  
The default value of this parameter is False.  
