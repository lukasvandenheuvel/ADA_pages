# What guides our political affiliations?
Ever since the dawn of democracies, political scientists have been searching for the fundamental questions that best define our political beliefs. Do you favour small or big state? Are you progressive or conservative? Authoritarian or liberal? Those were some of the questions traditionally deemed most important. These believes about what questions best characterise the political debate have been also captured graphically on graphs known as "political compasses" which show where different people lie on the questions defined above.

<!--This is a bit shit, replace by better image -->
![Example of traditional policital compass](https://2.bp.blogspot.com/-mj4BKwVVT0E/UyBQIwfMv3I/AAAAAAAACbs/bClT9FdMPgU/s1600/Social+democracy+2014.png "Example of traditional compass")

Traditionally, the axis on such compasses are along the lines left-right on one and authoritarian/libertarian on the other. But do these axes really accurately define the political divide today when traditional <!--Here we could add some example e.g. Conservatives in the UK raising taxes and giving out a lot of welfare when they were always a small-state party; democrats getting support from college-educated americans despite traditionally being a party of the working class (same with labour in the UK); rise of non-traditional parties such as En Marche in France or various parties (northern league, 5* movement) in Italy that have largely replaced the traditionally dominant christian democrats;etc--> political affiliations are shifting and traditional sticking points no longer hold? Let's leverage the almost 180 milion quotes available in quotebank to find out! 


# What topics dominate the political debate?
Let's start our analysis with extracting only Americans' politicians' quotes from our quote database. We decided to focus only on the US to reduce the impact of local, country-specific topics. After filtering with said criteria, we are left with 9.5 million quotes from 14 thousand politicians <!--Maybe add a comment about why 14k is ok because it sounds like a LOT-->. Let's now have a look at what it is that these politicians talk about – but before we do, let's see who they are!

#### The Silent Majority
Looking at the politicians with the most quotes, we can see what statisticians call a "power law", also known as the 80-20 rule, i.e. few most quoted politicians completely dominate the debate. The most quoted politician (Donald Trump) alone accounts for almost 10% of the quotes (7.5% exactly). To demonstrate just how dominant this is, consider that as we have 14 thousand politicians, an average politician only accounts for 0.007 % of the quotes! Indeed, this data even trumps the 80-20 rule as the top 20% of politicians account for 88% of the quotes. This shows that in today's world, few of the loudest politicians occupy the vast majority of media coverage while the vast majority of politicians are given little attention – hence, the idea of a "silent majority" seems to be well supported by the evidence! <!-- Perhaps better description of what silent majority is is necessary -->

![Quote distribution shows strong dominance of loudest politicians](https://via.placeholder.com/800x300?text=Placeholder+Image "Loudest policitians dominate debate")

#### Dominant Topics





















See our Milestone 2 submission [here](milestone2.md).

# Introduction  
The search for political spectrum, i.e. a set of independent political dimensions which enable characterization of political positions in relation to one another, has long been a focus of political science research. While most commonly used models are primarily based on the left/right division dating all the way from the French Revolution, many political scientists argue it no longer accurately characterizes the political divisions of today ([1](https://www.perlego.com/book/532600/beyond-liberal-and-conservative-reassessing-the-political-spectrum-pdf), [2](https://ideas.repec.org/p/osf/socarx/tr8g5.html)). In this project, we propose to create a political spectrum empirically by leveraging the Quotebank dataset ([3](https://dl.acm.org/doi/10.1145/3437963.3441760)). Using topic and sentiment extraction applied to recent quotes of American politicians on the federal level, we will obtain their sentiments on current issues and perform dimensionality reduction to find the most divisive axes. Further analysis and interpretation of the resulting vector space will allow us to redefine the political spectrum based on the most contentious issues.  

# Add plotly commit


<div style="text:align: center">
  <iframe src="pca_opinions.html" height="525" width="800"></iframe>
</div>



<!---
### Markdown

<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://raw.githubusercontent.com/lukasvandenheuvel/ALAN/gh-pages/assets/images/pca_opinions.html" height="525" width="100%"></iframe>

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/lukasvandenheuvel/ADA_pages/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

-->
