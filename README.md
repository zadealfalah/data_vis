For this project I have chosen to use some NYPD crime data (something which was utilized in a previous course in this Masters programme).  I chose this data because while I got a basic look at it in the previous course I did not feel as though my visualisations that I created were very nice and I wanted to improve it even before I had signed up for this course.  It was also a very interesting and deep data set that is nicely cleaned up with more than enough data points for the project at hand.  While I forwent my previous analysis in favor of more high-level overviews in this, it will serve as a nice starting point for refreshing my previous work and sprucing it up into something I could put on a resume.  With all that said I would like to move through the three discussion prompts from the three weeks and follow it up with my current completed visualisations.

To begin with in week 1 we were asked to find our data and describe its source, key attributes,and our goals with the data- as well as to find relevant visualizations to critique.  As mentioned already I chose some NYPD crime data to work with.  This data can be downloaded from https://catalog.data.gov/dataset/nypd-shooting-incident-data-historic
My goals for working with this data were to create a nice, easy to use visualization tool which would allow anyone to come and see crime trends within NYC and tailor these data to their specific circumstances.  That is to say I wanted the user to be able to direct which data might be most useful to them and have my visualization display just that.  The key attributes that I chose to keep from this dataset were crime occurrence dates, occurrence times, boro locations, and victim metadata.  I had also thought of keeping perpetrator data and murder flag metadata but as of now I am skipping the use of them, though perhaps future iterations could add on the murder flag information.  This will be discussed more later.
While looking at preexisting NYC crime data visualizations I stumbled upon the following page: https://towardsdatascience.com/analysis-of-nyc-reported-crime-data-using-pandas-821753cd7e22
This individual happened to create some visualizations which were very similar to the type I was hoping to create and as such I chose these to critique.  To begin with  their ‘level of offense’ pie chart seems to have some very unpronounced 3-D effect which you can see most clearly near the bottom left hand of the chart.  Since 3-D should only be used when absolutely necessary, and can easily distort pie-chart readings, this seems unnecessary.  Especially since it is so minute that it’s hard to tell it’s there.  Additionally the pie chart adds to 100.1% which again is not too egregious an error, but it was explicitly mentioned in class that pie charts should always sum to exactly 100%.  The following line chart entitled ‘Total Crime Events by Year’ has a problem in that its Y-axis does not start at 0, something which was stressed to be important in our lectures.  This could easily be fixed by changing the graph to be one of percent change in crime event counts by year which shows the most pertinent information of that chart much more cleanly.  There are many more visualizations on this page all of which look at summarizing crime statistics within NYC.  While this is quite similar to what I want to do, it is lacking in the specific area that I wish to focus on- user specificity.  Seeing large scale data like these presented is interesting and fun to look at but does not have much bearing on an individuals’ day-to-day.  What I want to do is create a visualization that might help someone who is hoping to visit NYC stay safe.  As such I would want to make the graphs more tailored to the individual in question which seems most easily done by allowing some interactive filtering to occur.  
In week 2 we were asked to answer the following questions:
Why is a task pursued? (goal)
How is a task conducted? (means)
What does a task seek to learn about the data? (characteristics)
Where does a task operate? (target data)
When is the task performed? (workflow)
Who is executing the task? (roles)

To answer these in order:
Why: To allow the individual to better explore the data at a high level and to get a good idea of general trends of crime over time.  Primarily a presentation of the data so as to create the lowest possible barrier to entry, but with some basic interactivity (via drop-down menus) to allow the data to be best tailored to the individual and to keep them engaged.  
How: Again the use of basic interactivity will hopefully keep the user more engaged and allow them to access the more pertinent information from the data instead of slogging through the highest-level views.  Data trends within demographics seem more useful than overall crime trends.
Data characteristics: Higher-level data trends within the selected filters are the primary focus.  No need to try to force people to find the maxima or minima when a general trend does just as well for a fun, easy to use tool.
Target data: This data visualization will use the absolute reference frame of time and space (when and in which boro crimes occur) as well as some relative frames of comparing trends between boros or between victim sexes.
Workflow: Before selecting from the dropdowns there are the highest level data trends to see, which would hopefully lead to questions of the type like ‘would this change if I were going to borough X?  What about borough Y?  Do more crimes happen to women in this specific borough or to men?’.  This is where the simple dropdown menus allow for greater specificity in the data presented.
Roles: This tool is meant to be used by anybody who wishes to visit NYC and wants to see some higher-level crime trends so as to better stay safe.  As such there are hopefully no barriers to use for this tool other than a want to see such data and the ability to reason about general trends from basic line graphs.  Everything is kept as simple as possible so as to facilitate this general use case.
Some low-fidelity prototypes were created by following the five design sheets methodology which will be shown later.  
In week 3 we were asked to answer the following questions:
What is our target question
Who should we recruit to answer that question
What measures should be used and what do these measures say about our question
How will we answer the question
How will we instantiate our methods
What criteria are used to indicate a successful visualization 
The answer to these are as follows:
The target question is where and when is most safe in NYC and for whom.  
The people I would like to recruit would preferably be a large, randomized sample of individuals as I would like for this to be a tool anyone interested in traveling to NYC can use.  Since this is not feasible for this course I simply asked a colleague, a family member, and a friend in hopes of getting a wider (although clearly biased) sample of opinions
The measures to use would be generally qualitative.  For example how much users felt they learned, if it was applicable to them, if they’d use it as a reference, how long it took them to fit the data to themselves, intuitiveness of the tool, etc.
The approach to answering these would again be inherently qualitative.  Thinkalouds would be nice so as to see exactly what users do with the tool, if it’s genuinely intuitive for them or if they needed to be guided, etc.  Unfortunately since schedules did not line up I instead sent questions of the like from answer (3) above to them and had them fill it out survey style.
To actually answer these questions I would want to give them the most current version of the visualization tool and have them play around with it, speaking aloud about what they were thinking and any questions they had while doing so.  Since I was unable to conduct a thinkaloud I instead sent out survey questions asking for qualitative feedback as mentioned above.
The visualization would be successful if people could use it easily, had some fun with it, and may use it again.  Bonus points if someone genuinely used it for timing their personal trip to NYC.

When actually designing my product I utilized the five design sheets methodology beginning with a brainstorming in which I thought of the concept of a more customizable view of crime statistics since the usual way such statistics are shown are more big-picture and don’t mean much to the day-to-day of an individual.  I thought to look at crime statistics filtered interactively by the location the individual was planning to be, and their personal characteristics e.g. their sex, age, etc.  A dropdown to filter the data to show only crime statistics which occured to their specific demographic would then be used to cater results to the user.  Using the five design sheets methodology I then created low-fidelity prototypes of possible visualizations to use pictured below:


---SEE altair_male_selected_no_boro.png

These rough sketches included a bar chart which showed relative crime statistics for male and female individuals by boro, and two line charts which would show the number of incidents over time (one by time of year, the other by time of day) with each line representing a different boro.  Underneath of which was a drop-down selector which would allow the user to choose which boro to focus on and which gender they wanted the crime statistics for.  These were worked up quickly in python and then sent out to some others to get feedback on which seemed the most interesting and what they’d like more of.  After getting feedback the bar plot was scrapped and the two line graphs were merged into one visualization then sent back out to be reassessed.  At this time there were multiple dropdown selection tools including the individuals’ sex, age (binned), and the borough in question.  While these three seemed to work nicely together it was decided by majority vote that it was too much to care about at once and as such the age binning was removed and the two time scales (by time of year and time of day) were to be separated.  This leads us to the final product which has these two plots side by side and piped together so that selections from the dropdowns of the borough in question and gender of the individual effects both plots allowing for greater customization without overwhelming the user with the number of decisions to make.  A picture of this final product without a borough selected is shown here:





And if we were to instead select to show only incidents which occurred to women within the Bronx we would see instead:


---SEE altair_male_selected_one_boro.png


In one of the prototype iterations these two graphs shared a Y-axis so as to keep scale consistent which was mentioned in lecture.  As you can see here this did not make the final cut as testers complained that it made the graph too difficult to see clearly (especially for Staten Island which had so little data comparatively) .  As a compromise a re-labeling was decided upon since the primary focus of this tool was ease of use.  Since the new labels are explicit and prominent, and the general trends are more readable, it seems to have been the proper choice for this project.  
This final product follows the general workflow of an interactive visualization by beginning with an overview of the data trends as a whole, allowing for a filtering of the pertinent data, and finally having the details on demand via a mouse-over which displays the currently selected boro and sex.  It also follows the overview+detail focus mentioned in lecture by showing the large-scale temporal trends on the left next to smaller scale and more focused trends on the right.  The visualization allows for an iterative building up of knowledge in the same way beginning with a basic understanding of ‘this prompt should help show when it’s safe in NYC for you’, seeing the large-scale trends, then focusing in on the more specific questions such as ‘what about borough X?’ or ‘what about for women specifically?’.  By removing other interactive options but leaving these it should promote the building of the knowledge that we want, that is the times and places where NYC is the safest for the user in question.  These insights should be quick to find, and will hopefully be deeper than those that might be found from other comparable visualizations since these can be conformed to specific locations and for specific demographics (in this case borough and sex).  It should also hopefully provide some unexpected insights.  For example the basic fact that crimes tend to spike around July or August was already surprising for me, as well as the incredibly low number of reported crimes in Staten Island.  While I wasn’t expecting it to have higher numbers than say Brooklyn, it still did seem like not as much as I would have guessed.  The colors were chosen to be unrelated to show the different boroughs should not be accidentally grouped together as might happen with a gradient color scheme.  
I think that for future work some simple additions such a secondary graph in which similar data is shown but with line opacity being tied to the percentage of crimes which carried a positive ‘statistical murder flag’ could be quite interesting as a measure of relative safety of the area at a given time.  Additionally I would like to find a way to add more customization options such as the previously mentioned age bins as I feel like these are the things which set this visualization apart from a generic crime statistics line graph.  It would require some workshopping with multiple test users to find a way to include these without giving the users a feeling of being crowded with options.  Additionally I think that searching through more color schemes would be useful as there aren’t many colors needed here but having distinct, fun to look at colors which do not lend themselves easily to being misconstrued as grouped together could improve the look of the tool.  As of now though it fills its niche of being a simple, easy to use, and fun little tool for seeing relative safety by time and location for an individual within NYC.

