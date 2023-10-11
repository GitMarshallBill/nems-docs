NEMS Anonymous Stats
====================

NEMS Linux sends anonymous, non-confidential usage data to the NEMS
Linux Stats API. This data is aggregated by our system in a non-unique,
entirely anonymous way.

.. Note:: To ensure the privacy of our users' data, none of the data
   collected is identifying, nor is it even private information. We
   do not receive nor store any account information, passwords or the
   like.

The data included in the anonymous stats contain:

-  Which platform you're running NEMS Linux on,
-  How many hosts you have configured,
-  How many services you have configured,
-  Your NEMS Linux version,
-  The size of your NEMS Linux storage medium (E.G., SD card),
-  How much free space you have on that same medium,
-  Your NEMS Linux server average system load,
-  Your NEMS Linux server uptime,
-  Your NEMS Linux server CPU temperature.

In order to uniquely, but anonymously identify your NEMS Linux server
(E.G., so we do not duplicate data if you send it twice and so others
cannot pretend to be you) your NEMS Linux server will also provide us
with your NEMS Linux API Key (which it generates automatically) as well as
your NEMS Linux Hardware ID, which you can see within `NEMS Server
Overview <../apps/serveroverview.html>`__.

We store this information to give us an idea how many people are using
NEMS Linux, how many hosts they're monitoring, and how we can better improve
performance based on the information provided. We also provide an
aggregated stats display to help other users see the average performance
of each platform.

To see how this data is made publicly available, please visit the `NEMS
Linux Stats page <https://nemslinux.com/stats/>`__.

If you'd like to review what data we collect, please observe `the source
code <https://github.com/Cat5TV/nems-scripts/blob/master/stats.sh>`__ or
open `NEMS Server Overview <../apps/serveroverview.html>`__ on your
NEMS Server.
