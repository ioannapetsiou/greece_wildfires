# Wildfires in Greece 
## The data, notebooks, and process notes for project one
## What I aimed to accomplish:
With this project on Wildfires in Greece, besides practising my skills, I wanted to see how many acres have been burned in Greece from 2000 to 2023. Then, other questions rose, such as the the most affected regions, or the region that is affected most per year.
## My findings:
* From 2000 to 2023, a total of 12,266,940 acres have burned, equivalent to an area larger than the regions of Epirus or Western Macedonia. Greece’s total area is 131,957 km2, meaning nearly 10% of the country has been burned in this period.
* The region with the largest burned areas changes yearly, many regions have repeatedly ranked first for the highest number of burned acres.
* I also found the regions that have the most burned acres for the whole 2000 - 2023 period. The region with the most burned acres is Elis, then Evros, Evvoia and lastly Attica.
## Data collection process:
I used excel files that the Hellenic Fire Service [website](https://www.fireservice.gr/el/synola-dedomenon)) provides on their website. The first file includes all the years from 2000 to 2012. From 2013 and on, each year has its own excel file. I downloaded them and uploaded them one by one on a jupyter notebook.
## Data analysis process:
After uploading my excels on my jupyter notebook as dfs, I:
- setted the first row of the datasets as a header
- reseted the index
- turned the column "Ημερ/νία Έναρξης" as datetime type
- extracted the year
- summed the burned stremmata (which mean burned acres) for each category by year and district and calling it as a new dataframe
- and printed the final dataframe for the year

After I did this for each excel seperately, I combined them into one big dataframe. Then, I translated the greek words to English, created a new column that calculated the total burned acres, and went onto answering my questions: found which region had the most burned acres for each year, saw how many acres burn each year in all regions, calculated the total burned acres for the whole period, and then found what percentage of Greece has burned.

<i> Note: The graphs and the project talks about greek acres called "Stremma", equal to 1,000 square metres or approximately ¼ acre. The burned acres include Forests, Forest Areas, Groves, Grasslands, Reeds - Swamps, Agricultural Areas, Crop Residues and Landfills. </i>

In the files I uploaded, you can also find the datasets I created for Visualizations.
- <b> fires </b> : has the combination of all seperate datasets that I cleaned from the Hellenic Fire Service
- <b> nomoi </b>: has the region with most burned acres per year
- <b> nomoi_synolo_zhmias </b> : has the total number of acres burned per region
- <b> by_category </b> : has the acres that were burned each year for all regions, by category

## Where did I grow the most / What did I want to do but couldn't:
It was my first time working with greek data, and I had to translate that in English, so that I could make the graphs. I used a dictionary where I wrote the English name for all the greek regions that were on the dataset, but I suppose there is a library out there that could do this for me. I googled and found somethings around, but they didn't seem to work.

I also suppose <i> (and deep inside know) </i> that there is an other way to download all the excels at the same time through the website, and work on all of them at the same time? However, it felt safer to do it one by one, and since they weren't that many it wasn't really a problem.

I definitely got the chance to practise my skills, data and visualization wise. I made two vizualizations on flourish, and one map on DataWrapper.

## Website
You can fink the url for my website [here](https://ioannapetsiou.github.io/wildfires/)
