task one was worked by the Rwema Gisa
Rwema Gisa so the command to delete file test-1 is rm test-1
and move top5-highest-temperatures.csv to data directory  is mv "top5-highest-temperatures.csv" data/

task two was worked by the prince Mbonyumugisha and Promesse Irakoze

to Remove Duplicates: commad is -cat satelite_temperature_data.csv | sort | uniq -d
-sort satelite_temperature_data.csv | uniq > cleaned_satelite_temperature_data.csv

to Extract Top 5 Highest and Lowest Temperatures:

-cut -d ',' -f 2,1 cleaned_satelite_temperature_data.csv | sort -t ',' -k1,1nr | head -n 5 > analyzed/top-5-highest-temperatures.csv
-cut -d ',' -f 2,1 cleaned_satelite_temperature_data.csv | sort -t ',' -k1,1n | head -n 5 > analyzed/top-5-lowest-temperatures.csv

Extra Task: Extract data for your country

-grep 'YourCountry' cleaned_satelite_temperature_data.csv > analyzed/country-heat_data.csv

