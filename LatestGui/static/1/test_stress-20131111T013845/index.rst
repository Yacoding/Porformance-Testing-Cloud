======================
FunkLoad_ bench report
======================


:date: 2013-11-11 01:38:45
:abstract: Stress Testing on user supplied link
           Bench result of ``Stress.test_stress``: 
           Access (nb_time)s times the main url

.. _FunkLoad: http://funkload.nuxeo.org/
.. sectnum::    :depth: 2
.. contents:: Table of contents
.. |APDEXT| replace:: \ :sub:`1.5`

Bench configuration
-------------------

* Launched: 2013-11-11 01:38:45
* From: mayank
* Test: ``test_Stress.py Stress.test_stress``
* Target server: http://intranet.iiit.ac.in
* Cycles of concurrent users: [10]
* Cycle duration: 10s
* Sleeptime between request: from 0.0s to 0.5s
* Sleeptime between test case: 0.01s
* Startup delay between thread: 0.01s
* Apdex: |APDEXT|
* FunkLoad_ version: 1.16.1


Bench content
-------------

The test ``Stress.test_stress`` contains: 

* 2 page(s)
* 0 redirect(s)
* 1 link(s)
* 4 image(s)
* 0 XML RPC call(s)

The bench contains:

* 143 tests
* 292 pages
* 1025 requests


Test stats
----------

The number of Successful **Tests** Per Second (STPS) over Concurrent Users (CUs).

 .. image:: tests.png

 ================== ================== ================== ================== ==================
                CUs               STPS              TOTAL            SUCCESS              ERROR
 ================== ================== ================== ================== ==================
                 10             14.300                143                143             0.00%
 ================== ================== ================== ================== ==================



Page stats
----------

The number of Successful **Pages** Per Second (SPPS) over Concurrent Users (CUs).
Note that an XML RPC call count like a page.

 .. image:: pages_spps.png
 .. image:: pages.png

 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                CUs             Apdex*             Rating               SPPS            maxSPPS              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                 10              1.000          Excellent             29.200             34.000                292                292             0.00%              0.010              0.058              0.339              0.012              0.039              0.130              0.149
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

 \* Apdex |APDEXT|

Request stats
-------------

The number of **Requests** Per Second (RPS) successful or not over Concurrent Users (CUs).

 .. image:: requests_rps.png
 .. image:: requests.png

 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                CUs             Apdex*            Rating*                RPS             maxRPS              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                 10              1.000          Excellent            102.500            119.000               1025               1025             0.00%              0.004              0.018              0.219              0.006              0.014              0.034              0.040
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

 \* Apdex |APDEXT|

Slowest requests
----------------

The 5 slowest average response time during the best cycle with **10** CUs:

* In page 002, Apdex rating: Excellent, avg response time: 0.02s, get: ````
  `Get url`
* In page 001, Apdex rating: Excellent, avg response time: 0.02s, get: ````
  `Get url`
* In page 001, Apdex rating: Excellent, avg response time: 0.02s, image: ``/banner.jpg``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.02s, image: ``/pdficon.png``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.02s, image: ``/bottom.jpg``
  ``

Page detail stats
-----------------


PAGE 001: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ````

     .. image:: request_001.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                142                142             0.00%              0.010              0.019              0.067              0.011              0.018              0.029              0.032
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, link, url ``/index.css``

     .. image:: request_001.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                143                143             0.00%              0.005              0.016              0.054              0.005              0.011              0.032              0.046
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, image, url ``/banner.jpg``

     .. image:: request_001.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                146                146             0.00%              0.006              0.019              0.219              0.006              0.012              0.036              0.040
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 004, image, url ``/pdficon.png``

     .. image:: request_001.004.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                147                147             0.00%              0.007              0.018              0.067              0.008              0.013              0.035              0.041
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 005, image, url ``/newicon.gif``

     .. image:: request_001.005.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                148                148             0.00%              0.004              0.016              0.065              0.005              0.011              0.035              0.040
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 006, image, url ``/bottom.jpg``

     .. image:: request_001.006.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                149                149             0.00%              0.004              0.016              0.065              0.005              0.011              0.036              0.046
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

PAGE 002: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ````

     .. image:: request_002.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                     10              1.000          Excellent                150                150             0.00%              0.010              0.020              0.046              0.011              0.017              0.034              0.037
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

Definitions
-----------

* CUs: Concurrent users or number of concurrent threads executing tests.
* Request: a single GET/POST/redirect/xmlrpc request.
* Page: a request with redirects and resource links (image, css, js) for an html page.
* STPS: Successful tests per second.
* SPPS: Successful pages per second.
* RPS: Requests per second, successful or not.
* maxSPPS: Maximum SPPS during the cycle.
* maxRPS: Maximum RPS during the cycle.
* MIN: Minimum response time for a page or request.
* AVG: Average response time for a page or request.
* MAX: Maximmum response time for a page or request.
* P10: 10th percentile, response time where 10 percent of pages or requests are delivered.
* MED: Median or 50th percentile, response time where half of pages or requests are delivered.
* P90: 90th percentile, response time where 90 percent of pages or requests are delivered.
* P95: 95th percentile, response time where 95 percent of pages or requests are delivered.
* Apdex T: Application Performance Index, 
  this is a numerical measure of user satisfaction, it is based
  on three zones of application responsiveness:

  - Satisfied: The user is fully productive. This represents the
    time value (T seconds) below which users are not impeded by
    application response time.

  - Tolerating: The user notices performance lagging within
    responses greater than T, but continues the process.

  - Frustrated: Performance with a response time greater than 4*T
    seconds is unacceptable, and users may abandon the process.

    By default T is set to 1.5s this means that response time between 0
    and 1.5s the user is fully productive, between 1.5 and 6s the
    responsivness is tolerating and above 6s the user is frustrated.

    The Apdex score converts many measurements into one number on a
    uniform scale of 0-to-1 (0 = no users satisfied, 1 = all users
    satisfied).

    Visit http://www.apdex.org/ for more information.
* Rating: To ease interpretation the Apdex
  score is also represented as a rating:

  - U for UNACCEPTABLE represented in gray for a score between 0 and 0.5 

  - P for POOR represented in red for a score between 0.5 and 0.7

  - F for FAIR represented in yellow for a score between 0.7 and 0.85

  - G for Good represented in green for a score between 0.85 and 0.94

  - E for Excellent represented in blue for a score between 0.94 and 1.

Report generated with FunkLoad_ 1.16.1, more information available on the `FunkLoad site <http://funkload.nuxeo.org/#benching>`_.