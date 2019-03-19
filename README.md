# Around：a Geo-index based social network
This repo is the backend implementation of Around. You can view the front end impelentation at [here](https://github.com/wuhaoyujerry/Around-web).

## Project Detail
* Built a scalable web service in Go to handle posts and deployed to Google Cloud (GAE flex) for better scaling.
* Utilized ElasticSearch (GCE) to provide geolocation-based search functions such that users can search nearby posts within a distance (e.g. 200km).
* Used Google Dataflow to implement a daily dump of posts from BigTable to BigQuery table for offline analysis, including aggregating the data at the post level and user level to improve keyword-based spam detection.
* Used Google Cloud Storage to store media data such as images and videos.
* Used OAuth 2.0 to support authentication and user signup and Redis to improve cache performance.
