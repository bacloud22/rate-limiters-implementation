# rate-limiters-implementation
This is how rate limiters and throttlers should be implemented

![voila](Throttler.drawio.svg)

Let me add these assumptions

1- Note that the processing time can be naively calculated by the start of the request, and the time server returns result to client, however, for a more robust implementation, a rate limiter would add asynchronous processing time left behind, I know this is not easy, but maybe it worth time to invest.

2- Also anyway, the time a request needs to deliver, doesn't necessarily reflect the CPU being busy (maybe just fooling around or waiting) 😄 
