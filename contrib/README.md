# TOC in XML

wget "http://ec.europa.eu/eurostat/estat-navtree-portlet-prod/BulkDownloadListing?sort=1&file=table_of_contents.xml" -O table_of_contents.xml

xsltproc rdf + html

Now done in a test case to automatically update the table of contents files.

grep -e "ramon/nuts" nuts.html |  sed -e "s/.*ramon\/nuts\/\(\S*\)<\/a>/\1/g" | grep -ve "^  "