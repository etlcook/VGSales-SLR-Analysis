# README

## Changelog
08/03/2023: 
PR `fix-eda` addresses:
- You are only including systems that were produced after 2010, but excluded 3DS and PC games. I think you were just going for console platforms, but also included the PSVita (maybe you thought this was Playstation 5), in which case the 3DS and PC could be included.
*You're right, I misstook "PSV" to mean "PS5". However, I don't think it would be an issue to include portables and PC. New PR includes 3DS, PC Games*
* 		What are the units for the mean sales platform tables?
*Millions of units sold. The `aggregate()` function calculates the mean for the columns but the units remain the same*
* 		I already mentioned the total_sales_genre not existing when trying to knit
*Removed and refactored this section to be more simple*
* 		Are we going to remove observations with year of NA? I would think so right?
*Fixed; Removed < 2% of dataset where `Year` was "N/A" and cast `Year` to numeric datatype*
* 		It looks like there are very little observations after the year 2016 (less than 5), which is why the total_sales_year plot makes it look like the market crashed in 2017. No big deal but we can say the data is from 2010 to 2016 instead
*concur, we now filter the dataset at the very beginning to remove observations after 2016*

---