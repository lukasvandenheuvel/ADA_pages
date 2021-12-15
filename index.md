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

These topics are the ones which are most talked about, but are they also most divisive? Let's find out!

#### Divisive Topics
To analyze which topics divide politicians, we first need to get their sentiment towards each topic. For example, do they feel positive or negative towards Hillary Clinton or Womens' Rights? To do this, we used Vader, a tool which assigns a number from -1 (negative sentiment) through 0 (neutral sentiment) to 1 (positive sentiment) to each individual quote. This allowed us to get the sentiment of each politician for each topic [^2].

Then, we focused on the republican/democratic divide. On which topics do their sentiments differ the most? 

![Most divisive topics are transitory culture-war issues](https://via.placeholder.com/800x300?text=Placeholder+Image "Most divisive topics")

The analysis shows that most divisive topics are in fact not topics of long-term vision for the country but rather those relating to transient issues that we could label as part of "culture wars" – they are related to particular people who polarized the public debate such as Mike Pompeo and Mike Pence or former FBI director Jim Comey. Interestingly, a topic about former president Donald Trump is not present. The only long-term topic out of the most divisive ones is the 'Rejection of Paris accord' which unsurprisingly triggered positive sentiments from republicans. Another interesting finding is that 2 out of the top 10 most divisive topics are Trump-appointed Supreme Court Justices, Kavanaugh and Gorsuch, showing the politicization of the Supreme Court which has become a powerful player in a country with blocked legislature.
<!--{'920': 'Mike Pompeo','380': 'Mike Pence','558': 'Judge Neil Gorsuch','680': 'John Bolton','143': 'Kavanaugh family','208': 'FBI and Jim Comey','360': 'FISC, Adam Schiff','566': 'Rejection of Paris accord','615': 'Marco Rubio','841': 'Pittsburgh shooting'}-->


# Key Takeaways
- Few politicians completely dominate the public debate – **silent majority** phenomenom does exist!
- Topics politicians most talk about are not the ones where they most disagree – contrary to popular opinion, they agree on many issues!
- Topics that most divide politicians are mostly "culture wars" ephemeral topics that have little to do with a greater vision for the country.
- 

[^1]: Due to technical limitations, we used a subset of 600k quotes for the topic extraction and we then use BERTTopic to assign the remaining quotes to these topics. Also, we limited BERTTopic to 1000 topics as when left to its own devices, it would generate over 4000 topics where each topic was extremely narrow and provided little interpretation possibilities.

[^2]: In particular, we did this as follows: first we assigned a sentiment to all the quotes. Then, for each politician, we averaged the sentiment of their quotes to each topic. We then removed politicians with less than 1000 quotes as a lower number than that did not give us sufficient representation of their opinions. If politicians did not express an opinion towards a topic, we left their sentiment as NaN, eventually replacing it with 0 for some further processing.
