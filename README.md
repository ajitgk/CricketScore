# CricketScore
Basic angular based application that reads live cricket scores (json files) and displays the results. It currently uses raw html without any scheme or styling.

The live scores are pulled as JSON files (through http get method) from http://www.cricscore-api.appspot.com

1) To get details of all matches:
<br/>
<i>
 GET /csa HTTP/1.1
<br/>
 Host: cricscore-api.appspot.com
</i>

2) To get details of a single match:
<br/>
<i>
GET /csa?id=597924 HTTP/1.1 <br/>
Host: cricscore-api.appspot.com <br/>
If-Modified-Since:Sun, 30 Jun 2013 23:58:22 IST <br/>
</i>

3) To get details of more than one match:
<br/>
<i>
GET /csa?id=631136+585683 HTTP/1.1 <br/>
Host: cricscore-api.appspot.com <br/>
If-Modified-Since:Sun, 30 Jun 2013 23:58:22 IST<br/>
</i>

<b>TODO:</b>
<p>
1) Add html and css formatting <br/>
2) Update the live scores based on If-Modified-Since header parameter <br/>
3) Add ability to view scores for more than one match at a time <br/>
