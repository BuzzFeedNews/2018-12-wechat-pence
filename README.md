# Criticizing the Trump Administration on WeChat

This repository contains data and graphics supporting the BuzzFeed News article "[China’s Censors Give Anti-Trump And Anti-US Rhetoric A Pass On WeChat](https://www.buzzfeednews.com/article/craigsilverman/china-censor-trump-content-wechat)", published December 19, 2018.

## Data

The data in this repository comes from [WeChatscope](http://wechatscope.jmsc.hku.hk/), a project from Hong Kong University. It tracks and archives stories from a large, curated userbase of public and semi-public accounts in China. See WeChatscope's [documentation](http://wechatscope.jmsc.hku.hk/) for more information. 

## Search Methodology

BuzzFeed News collected WeChat data, via WeChatscope, for 744,671 posts created between April 1, 2018 and November 15, 2018.

WeChatscope records the title of each post in the original Mandarin. For our analysis of posts about Vice President Mike Pence, we searched for the following characters in the post title:

- "彭斯" ("Pence")
- "副总统" ("Vice President")

The search yielded 199 results. Two Mandarin speakers reviewed and summarized the posts. We removed eight unrelated posts. 

## Spreadsheet

The spreadsheet of stories related to Vice President Mike Pence is located in the `data` folder. It contains the following columns:

- **id**: A unique identifier.
- **archive**: A URL directing to an archive copy of the original WeChat post. If the post is censored, this archive link will still function.
- **censored_date**: The date WeChatscope noticed the post was censored and removed from WeChat, if applicable.
- **censored_msg**: The censorship message left on the post when it is removed.
- **created_at**: The date the post was created.
- **nickname**: The username of the creator of the post.
- **title**: The title of the post in Mandarin.
- **update_date**: The date WeChatscope's servers checked the post again for censorship, if applicable.
- **original_url**: The URL for the original WeChat post. 

## Weekly counts and chart

The Jupyter Notebook at `notebooks/calculate-and-chart-weekly-counts.ipynb` contains Python code to calculate the weekly number of WeChat posts refering to Pence. In the [story](https://www.buzzfeednews.com/article/craigsilverman/china-censor-trump-content-wechat), we use that data to chart the sudden increase in stories about Pence after his [speech](https://www.hudson.org/events/1610-vice-president-mike-pence-s-remarks-on-the-administration-s-policy-towards-china102018) at the Hudson Institute on October 4.

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). 

## Questions / Comments?

Please contact Scott Pham at scott.pham@buzzfeed.com.

Looking for more from BuzzFeed News?  [Click here for a list of our open-sourced projects, data, and code](https://github.com/BuzzFeedNews/everything)

