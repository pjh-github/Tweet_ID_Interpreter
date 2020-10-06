# Extract Date, Data centre, server and sequence ID from Tweets. 
Small script for decoding and parsing twitter tweet ids &amp; associated resources.

## Goal - Extract timestamp, datacenter, server and sequence from tweet ID.

### Assumptions -
This is accurate: https://twitter.com/conspirator0/status/1227063249440509952/photo/1
Tweets can be split up into the given structure.

### Methodology -

   - Extract tweet ID
   - Take URL e.g: https://twitter.com/realDonaldTrump/status/1226595698793230348
     Actual tweet date - 7:56 PM Feb 9, 2020
     Split by '/', take the final component
   - Convert to Binary
   - Substring binary into timestamp, datacenter, server and sequence. 
   - Pass to given timestamp logic.
   - Return timestamp and decimal conversion of datacenter, server and sequence.

More info here: https://developer.twitter.com/en/docs/basics/twitter-ids 

 ### Todo - 
 
 Hook up with this for some statistical analysis: https://github.com/hhromic/python-twitter-toolbox
