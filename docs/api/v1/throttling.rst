Throttling
==========

In order to keep the CIViC API reliable, free, and open to all, we maintain some basic rate limits on its usage.

The default rate limit is approximately 2 requests/second calculated over a 5 minute moving window. That means you may burst substantially higher than 2 requests/second for short periods.

If you are hitting the rate limit, you will get a ``429 Too Many Requests`` HTTP response. You will need to wait for that five minute window to elapse before making additional requests.

HTTP Headers
------------

CIViC provides information about the current rate limit and your progress towards it via headers in the HTTP response. The following headers are available:

.. list-table::
   :widths: 30 70
   :header-rows: 1

   * - Header Name
     - Description
   * - RateLimit-Limit
     - The total number of requests allowed in the time window
   * - RateLimit-Remaining
     - The number of requests you have remaining during the time window
   * - RateLimit-Reset
     - Time (seconds since the Unix Epoch) when the time window resets

Avoiding The Rate Limit In Scripts
----------------------------------

Here are several tips and techniques you can employ to stay under the rate limit.

.. rubric:: Delay/Sleep

If you know you’re going to be performing many requests over a sustained period of time, one of the simplest methods is to introduce a slight delay between requests. That will allow you to remain under the rate limit indefinitely and your script to run uninterrupted.

.. rubric:: Caching

Often we see many requests for the same entity repeated over and over. While CIViC data does update regularly, caching the result for a request for the duration of a script will help you stay under the rate limit and increase the performance of your script at the same time.

.. rubric:: Automated Backoff

The most surefire way to make sure you never get rate limited is to use the HTTP response headers documented above. Before your script makes another request, it can check the ``RateLimit-Remaining`` header and if it sees a 1 or 0, not make additional requests until ``RateLimit-Reset``. You can also wait to get a ``429`` status code, put in a similar delay and retry your request.

Reach Out To Us!
----------------

If you have a use case that isn’t being addressed, think you need an increased rate limit, or have questions about efficiently using the CIViC API, please `send an email to the civic-help email list <mailto:help@civicdb.org?subject=CIViC\ Help\ Request>`_ and we’d be happy to chat! Our goal is to keep the API freely accessible to everyone and not to limit usage as much as possible.
