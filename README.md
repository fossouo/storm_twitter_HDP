# storm_twitter_HDP
stream twets in storm (HDP 2.3)

1. Export JAVA_HOME
export JAVA_HOME=/usr/jdk64/jdk1.8.0_112

2. Build the project
mvn clean package

3. Run the Storm in either local or cluster Mode

storm jar target/tweet_loader-0.0.1-SNAPSHOT.jar  topologies.TweetTopology "[Your customer key]" "[Your secret key]" "[Your access token]" "[Your access secret]" "[Your NameNode]" "tweet-word-count"
