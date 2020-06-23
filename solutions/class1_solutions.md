# Solutions for Class 1

#### Write an algorithm/protocol/ruleset for making a PBJ sandwich.

1. Get out ingredients (peanut butter, jelly, bread).
2. Open peanut butter and jelly jars.
3. Lay two slices of bread on a plate.
4. Dip a butter knife into the peanut butter and spread on one slice of bread.
5. Wipe knife of a paper towel.
6. Repeat step 4 and 5 with jelly on the remaining slice of bread.
7. Stack bread slices so that the peanut butter and jelly sides are touching and enjoy.

Your protocol might not look *exactly* like this one and thats ok! The idea here is that writing specific rules or steps to create a pbj is fairly simple. I was able to write a comprehensive protocol in less than ten steps. We can think of other situations in software a protocol would follow a stepwise process like building a static webpage or analyzing a highly standardized dataset.

#### Write an algorithm/protocol/ruleset for determining if an email is spam

This might be considered somewhat of a trick question. The idea here is that there are way too many variations in spam emails to easily determine rules for removing them from your inbox. You absolutely *could* write a rudimentary ruleset for this task, however it is likely that you will have a large amount of false negatives and false positives. Additionaly, if spammers figure out what is in your ruleset they can easily work around your rules! 

This is where machine learning becomes incredibly useful. The machine is able to pick up on underlying patterns in spam emails and create a complex ruleset much faster and more accurately than a human brain. Further, you could continually train your machine learning algorithm on spam emails so it picks up the latest tricks that spammers are using to get around your system.
