# Table of Contents
- [Overview](#overview)
- [Metric Info](#metric-info)
- [User-Defined Parameters](#user-defined-parameters)
- [Reference](#reference)

# Overview <a name="overview"></a>
The API is used to retrieve the regional disk's replica state.

It leverages the GCP Cloud monitoring to fetch metrics of GCP resources via the GCP RESTful API. 

# Metric Info <a name="metric-info"></a>
* <b>Resource Label Used</b>: Unique identifier of the disk (disk_id).
* <b>GCP Original Name</b>: disk/regional/replica_state

# User-Defined Parameters <a name="user-defined-parameters"></a>
* <b>Start Time / End Time</b>: Define the time range to analyze data points, useful for historical analysis or recent monitoring. Default time range is the last 24 hours.


# Reference <a name="reference"></a>
* <b>Metrics Details</b>: https://cloud.google.com/monitoring/api/metrics_gcp
* <b>Metrics API</b>: https://cloud.google.com/monitoring/api/v3/filters