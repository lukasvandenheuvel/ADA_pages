# What guides our political affiliations?
Ever since the dawn of democracies, political scientists have been searching for the fundamental questions that best define our political beliefs. Do you favour small or big state? Are you progressive or conservative? Authoritarian or liberal? Those were some of the questions traditionally deemed most important. These believes about what questions best characterise the political debate have been also captured graphically on graphs known as "political compasses" which show where different people lie on the questions defined above.

<!--This is a bit shit, replace by better image -->
![Example of traditional policital compass](https://2.bp.blogspot.com/-mj4BKwVVT0E/UyBQIwfMv3I/AAAAAAAACbs/bClT9FdMPgU/s1600/Social+democracy+2014.png "Example of traditional compass")

Traditionally, the axis on such compasses are along the lines left-right on one and authoritarian/libertarian on the other. But do these axes really accurately define the political divide today when traditional
<!--Here we could add some example e.g. Conservatives in the UK raising taxes and giving out a lot of welfare when they were always a small-state party; democrats getting support from college-educated americans despite traditionally being a party of the working class (same with labour in the UK); rise of non-traditional parties such as En Marche in France or various parties (northern league, 5* movement) in Italy that have largely replaced the traditionally dominant christian democrats;etc-->
political affiliations are shifting and traditional sticking points no longer hold? Let's leverage the almost 180 milion quotes available in quotebank to find out! 

# What dominates the political debate?
Let's start our analysis with extracting only Americans' politicians' quotes from our quote database. We decided to focus only on the US to reduce the impact of local, country-specific topics. After filtering with said criteria, we are left with 9.5 million quotes from 14 thousand politicians <!--Maybe add a comment about why 14k is ok because it sounds like a LOT-->. Let's now have a look at what it is that these politicians talk about – but before we do, let's see who they are!

#### The Silent Majority
Looking at the politicians with the most quotes, we can see what statisticians call a "power law" (commonly also known as the 80-20 rule) i.e. few most quoted politicians completely dominate the debate. The most quoted politician (Donald Trump) alone accounts for almost 10% of the quotes (7.5% exactly). To demonstrate just how dominant this is, consider that as we have 14 thousand politicians, an average politician only accounts for 0.007 % of the quotes! Indeed, our data even trumps the 80-20 rule as the top 20% of politicians account for 88% of the quotes. This shows that in today's world, few of the loudest politicians occupy the vast majority of media coverage while the vast majority of politicians are given little attention – hence, the idea of a "silent majority" seems to be well supported by the evidence! <!-- Perhaps better description of what silent majority is is necessary -->

![Quote distribution shows strong dominance of loudest politicians](https://via.placeholder.com/800x300?text=Placeholder+Image "Loudest policitians dominate debate")

#### Dominant Topics
Having examined the politicians behind the quotes, let's investigate their content. To do this, we use a tool called BERTTopic to extract the topics that best characterise the quotes, which leads us to the top 1000 most significant topics [^1]. Of course, 1000 topics is a bit too many to interpret and to create a political compass, we will need to reduce this down further. But before we do, let's get some idea about what the most significant topics are!

To do this, we look at the quotes that BERTTopic finds as best representatives of the topics it found. Amongst the top 10 topics with most quotes, many are uncannily familiar: the most common topic is Hillary Clinton, others among the top 10 include Iran, Womens' Rights, Taxation or Youth.

> We have to tell young people that it does matter, every vote counts!
> 
> – <cite> Most representative quote for the "Youth" topic </cite>

[^1]: Due to technical limitations, we used a subset of 600k quotes for the topic extraction and we then use BERTTopic to assign the remaining quotes to these topics. Also, we limited BERTTopic to 1000 topics as when left to its own devices, it would generate over 4000 topics where each topic was extremely narrow and provided little interpretation possibilities.
