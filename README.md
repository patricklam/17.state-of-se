# Build instructions

I found that the previous build was accounting for 20k files and pentupling my Hugo build time. Hugo's supposed to be fast!

It looks like I can use revelry even though it hasn't been updated for a while. Yay Docker.

```$ docker run -v $(pwd):/work -u $(id -u) fishpercolator/revelry build```

Then I copy the www directory to my static directory. I did have to run ```revelry upgrade``` first.
