Telegram Scanner is a hacked credentials scanner that will scan telegram for hacked credentials, stealer logs, hacked databases, etc and build a Postgres DB with all the hacked information in it. 

It will start with a bot that will download and scrape the files from telegram servers, then they will be parsed and downloaded into the composite credentials and related information. Then it will be stored in the central Postgres DB (possibly with caching or other such optimizaitons). This is a heavily threadable process so that could be used.

Once in the DB indexing and searchability is added along with analytics and other such features to develop a deep insight into the hacked credentials web. Some examples are seeing where a email is reused, or a password, or a substring in passwords. Or what other breaches a certain website's breach appears in (like what cross pollenation userbase spread).

This tech stack can be done in Python / Go for the backend (Maybe rust for speed optimizations) and JS or Rust for the front end.

The goal is to allow blue teamers to have deeper insight into the network of hacked credentials and red-teamers to see how they are affected by breaches. Also just for general data exploration and insight.