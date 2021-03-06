======================
FunkLoad_ bench report
======================


:date: 2013-11-21 14:51:57
:abstract: Stress Testing on user supplied link
           Bench result of ``Stress.test_stress``: 
           Access (nb_time)s times the main url

.. _FunkLoad: http://funkload.nuxeo.org/
.. sectnum::    :depth: 2
.. contents:: Table of contents
.. |APDEXT| replace:: \ :sub:`1.5`

Bench configuration
-------------------

* Launched: 2013-11-21 14:51:57
* From: artoo
* Test: ``test_Stress.py Stress.test_stress``
* Target server: http://search.iiit.ac.in/courses
* Cycles of concurrent users: [5, 10]
* Cycle duration: 5s
* Sleeptime between request: from 0.0s to 0.5s
* Sleeptime between test case: 0.01s
* Startup delay between thread: 0.01s
* Apdex: |APDEXT|
* FunkLoad_ version: 1.16.1


Bench content
-------------

The test ``Stress.test_stress`` contains: 

* 5 page(s)
* 10 redirect(s)
* 2 link(s)
* 2 image(s)
* 0 XML RPC call(s)

The bench contains:

* 1 tests
* 133 pages
* 193 requests


Test stats
----------

The number of Successful **Tests** Per Second (STPS) over Concurrent Users (CUs).

 .. image:: tests.png

 ================== ================== ================== ================== ==================
                CUs               STPS              TOTAL            SUCCESS              ERROR
 ================== ================== ================== ================== ==================
                  5              0.200                  1                  1             0.00%
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
                  5              1.000          Excellent             12.600             18.000                 63                 63             0.00%              0.013              0.305              1.412              0.018              0.037              0.891              1.351
                 10              0.927               Good             14.000             29.000                 70                 70             0.00%              0.020              0.568              2.282              0.024              0.065              2.022              2.057
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
                  5              1.000          Excellent             16.600             30.000                 83                 83             0.00%              0.013              0.231              1.201              0.019              0.041              0.882              1.060
                 10              0.927               Good             22.000             35.000                110                110             0.00%              0.020              0.361              2.119              0.026              0.063              1.703              1.759
 ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

 \* Apdex |APDEXT|

Slowest requests
----------------

The 5 slowest average response time during the best cycle with **10** CUs:

* In page 001, Apdex rating: POOR, avg response time: 1.80s, get: ``/courses/www/index.php``
  ``
* In page 002, Apdex rating: FAIR, avg response time: 1.53s, get: ``/courses/www/index.php``
  ``
* In page 003, Apdex rating: Excellent, avg response time: 0.20s, get: ``/courses``
  `Get url`
* In page 001, Apdex rating: Excellent, avg response time: 0.09s, link: ``/courses/www/themes/modern/css/css_global.css?build=11018``
  ``
* In page 001, Apdex rating: Excellent, avg response time: 0.07s, link: ``/courses/www/themes/default/images/favicon.png``
  ``

Page detail stats
-----------------


PAGE 001: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ``/courses``

     .. image:: request_001.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  3                  3             0.00%              0.026              0.034              0.047              0.026              0.028              0.047              0.047
                     10              1.000          Excellent                  4                  4             0.00%              0.051              0.058              0.068              0.051              0.059              0.068              0.068
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/courses/``

     .. image:: request_001.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  4                  4             0.00%              0.019              0.039              0.051              0.019              0.049              0.051              0.051
                     10              1.000          Excellent                  6                  6             0.00%              0.052              0.073              0.089              0.052              0.085              0.089              0.089
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, get, url ``/courses/www/index.php``

     .. image:: request_001.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              1.060              1.122              1.201              1.060              1.088              1.201              1.201
                     10              0.500               POOR                 10                 10             0.00%              1.679              1.796              2.119              1.703              1.759              2.119              2.119
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 004, link, url ``/courses/www/themes/default/images/favicon.png``

     .. image:: request_001.004.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.030              0.046              0.060              0.030              0.041              0.060              0.060
                     10              1.000          Excellent                 10                 10             0.00%              0.025              0.073              0.156              0.030              0.066              0.156              0.156
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 005, link, url ``/courses/www/themes/modern/css/css_global.css?build=11018``

     .. image:: request_001.005.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.078              0.106              0.138              0.078              0.096              0.138              0.138
                     10              1.000          Excellent                 10                 10             0.00%              0.059              0.089              0.109              0.063              0.094              0.109              0.109
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 006, image, url ``/courses/www/themes/default/images/logo/siel-logo-transparent.png``

     .. image:: request_001.006.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.047              0.063              0.099              0.047              0.057              0.099              0.099
                     10              1.000          Excellent                 10                 10             0.00%              0.028              0.056              0.071              0.033              0.063              0.071              0.071
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 007, image, url ``/courses/www/themes/default/images/others/transparent.gif``

     .. image:: request_001.007.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.021              0.032              0.041              0.021              0.036              0.041              0.041
                     10              1.000          Excellent                 10                 10             0.00%              0.026              0.043              0.066              0.026              0.041              0.066              0.066
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

PAGE 002: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ``/courses``

     .. image:: request_002.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.019              0.031              0.047              0.019              0.033              0.047              0.047
                     10              1.000          Excellent                 10                 10             0.00%              0.020              0.034              0.050              0.023              0.032              0.050              0.050
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/courses/``

     .. image:: request_002.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.020              0.034              0.053              0.020              0.031              0.053              0.053
                     10              1.000          Excellent                 10                 10             0.00%              0.020              0.028              0.039              0.021              0.026              0.039              0.039
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, get, url ``/courses/www/index.php``

     .. image:: request_002.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.318              0.731              0.888              0.318              0.795              0.888              0.888
                     10              0.700               FAIR                 10                 10             0.00%              1.284              1.525              1.768              1.396              1.520              1.768              1.768
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

PAGE 003: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ``/courses``

     .. image:: request_003.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.014              0.024              0.037              0.014              0.019              0.037              0.037
                     10              1.000          Excellent                 10                 10             0.00%              0.025              0.201              0.554              0.033              0.105              0.554              0.554
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/courses/``

     .. image:: request_003.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.013              0.031              0.070              0.013              0.024              0.070              0.070
                     10              1.000          Excellent                 10                 10             0.00%              0.026              0.062              0.176              0.031              0.039              0.176              0.176
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, get, url ``/courses/www/index.php``

     .. image:: request_003.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.359              0.700              0.891              0.359              0.700              0.891              0.891
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

PAGE 004: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ``/courses``

     .. image:: request_004.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.016              0.034              0.059              0.016              0.029              0.059              0.059
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/courses/``

     .. image:: request_004.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  5                  5             0.00%              0.024              0.029              0.037              0.024              0.028              0.037              0.037
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, get, url ``/courses/www/index.php``

     .. image:: request_004.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  4                  4             0.00%              0.707              0.787              0.897              0.707              0.811              0.897              0.897
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|

PAGE 005: Get url
~~~~~~~~~~~~~~~~~

* Req: 001, get, url ``/courses``

     .. image:: request_005.001.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  3                  3             0.00%              0.018              0.029              0.042              0.018              0.026              0.042              0.042
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 002, get, url ``/courses/``

     .. image:: request_005.002.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  3                  3             0.00%              0.016              0.019              0.020              0.016              0.020              0.020              0.020
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================

     \* Apdex |APDEXT|
* Req: 003, get, url ``/courses/www/index.php``

     .. image:: request_005.003.png

     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                    CUs             Apdex*             Rating              TOTAL            SUCCESS              ERROR                MIN                AVG                MAX                P10                MED                P90                P95
     ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ================== ==================
                      5              1.000          Excellent                  1                  1             0.00%              0.736              0.736              0.736              0.736              0.736              0.736              0.736
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