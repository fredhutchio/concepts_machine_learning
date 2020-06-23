## Solutions for Class 1

### Write an algorithm/protocol/ruleset for making a PBJ sandwich.

1. Get out ingredients (peanut butter, jelly, bread).
2. Open peanut butter and jelly jars.
3. Lay two slices of bread on a plate.
4. Dip a butter knife into the peanut butter and spread on one slice of bread.
5. Wipe knife of a paper towel.
6. Repeat step 4 and 5 with jelly on the remaining slice of bread.
7. Stack bread slices so that the peanut butter and jelly sides are touching and enjoy.

Your protocol might not look *exactly* like this one and thats ok! The idea here is that writing specific rules or steps to create a pbj is fairly simple. I was able to write a comprehensive protocol in less than ten steps. We can think of other situations in software a protocol would follow a stepwise process like building a static webpage or analyzing a highly standardized dataset.

### Write an algorithm/protocol/ruleset for determining if an email is spam

1. If an email is addressed to the wrong name it is spam.
2. If an email has x many typos it is spam.
3. If an email is from x, y, z people it is spam.
4. ...

This might be considered somewhat of a trick question. The idea here is that there are way too many variations in spam emails to easily determine rules for removing them from your inbox. You absolutely *could* write a rudimentary ruleset for this task, however it is likely that you will have a large amount of false negatives and false positives. Additionaly, if spammers figure out what is in your ruleset they can easily work around your rules! 

This is where machine learning becomes incredibly useful. The machine is able to pick up on underlying patterns in spam emails and create a complex ruleset much faster and more accurately than a human brain. Further, you could continually train your machine learning algorithm on spam emails so it picks up the latest tricks that spammers are using to get around your system.

### If we are trying to predict whether or not an animal is a cat or a dog what features might we collect?

Below are a list of some of the features you could collect:
* Head width
* Body length
* Tail length
* Weight
* Height

### Are there any cases you can think of that might confuse your algorithm based on the features you've chosen?

Yes! Cats and dogs that are outliars in their groups with regard to size and weight will throw off this algorithm. Further, small dogs are likely to get confused with cats.

<p align="center">
  <img src="https://pictures-of-cats.org/wp-content/uploads/2018/06/another-big-maine-coonB.jpg" width="300" />
  <img src="https://www.thesprucepets.com/thmb/SlxjoBXUHc48_GEgpuM0Taq7wIM=/1080x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/51152221_1137081246458617_3144049680416140765_n-5c73f04d46e0fb0001835dd2.jpg" width="300" />
</p>
