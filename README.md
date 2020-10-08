# NPS-Essential-Traveler-Information

### Project Summary

In 2016, NPS and USDOT Volpe Center created the [NPS National Long Range Transportation Plan (NLRTP)](https://rosap.ntl.bts.gov/view/dot/32531). This effort proposed a number of goals, objectives, and performance measures that would support the 20-year strategic direction and planning of NPS national parks and other public lands.

One goal area is to maintain and enhance the quality of visitor experience. The objectives under this goal are:
- Improve ease of access to and within national park units for all people
- Create a range of appropriate transportation options that support a network of seamless connections within each park unit and to surrounding communities
- Provide state-of-the-art traveler information and wayfinding and, where appropriate, interpretation and education opportunities that complement transportation options

NPS park unit websites can have major influence on visitors and their planning for visiting a park. NPS created nine essential pieces of traveler information that answer important questions for some groups of visitors (i.e. where is the parking? How do I get to the major sites? Can I take public transportation? Is it accessible?)

### Approach

The historical approach for this type of task is to have people manually look through websites for the related information. This approach can work for smaller tasks, but there are over 400 NPS park units with websites to monitor. This is likely too lofty a task for a consistent and timely results at the end.

This Github repo contains Python code that will scrape all the NPS websites, score on the essential elements for visitors, and create a final Excel sheet with the final scores. 

### Analytical Methods

Code can be found in two files:

1. **VE_scraper_functions.py**: This file has functions for scraping the different "Planning your visit" parts of each NPS website and classifying/scoring the parks for the essential elements.  
2. **NPS Site Scrape.ipynb**: This is a jupyter notebook where the park information is loaded and the functions are run, with quality checks.

Note on the NPS site scraping: This function does not do a fully exhaustive scrape, but instead goes 2 links from the NPS park home page. An alternative method might involve going to every possible site with the scraper. However, as we are thinking that this is made for visitors, we want to make sure people can easily access the information, so 2 clicks seemed appropriate.
