# Table of Contents
- [Overview](#overview)
- [Metric Info](#metric-info)
- [User-Defined Parameters](#user-defined-parameters)
- [Use Cases Example](#example)
    - [Use Case 1 -- Service Maintenance or Scaling Issues](#example-1) 
    - [Use Case 2 -- Load Balancer Performance Monitoring](#example-2)
- [Reference](#reference)

# Overview <a name="overview"></a>
The <b>HTTPCode_ELB_503_Count</b> metric tracks the number of HTTP 503 error codes generated by the load balancer. HTTP 503 errors indicate that the load balancer is unable to handle the request due to temporary overload or maintenance of backend services. Monitoring this metric helps detect when the load balancer or backend services are overwhelmed, preventing requests from being processed successfully.

# Metric Info <a name="metric-info"></a>
* <b>Metric Name</b>: HTTPCode_ELB_503_Count   
* <b>Namespace</b>: AWS/ApplicationELB
* <b>Unit</b>: Count
* <b>Display Name in NetBrain</b>: HTTP Code ELB 503 Count

# User-Defined Parameters <a name="user-defined-parameters"></a>
* <b>Start Time / End Time</b>: Specify the time range for viewing data points. This is useful for historical analysis or monitoring recent trends. The default time range is the last 24 hours.
* <b>Statistics</b>: Default value is Sum.
  * <b>Average</b>: The average number of HTTP 503 errors during the time period.
  * <b>Sum</b>: The total number of HTTP 503 errors returned by the load balancer.
  * <b>Minimum</b>: The least number of 503 errors in the selected period.
  * <b>Maximum</b>: The maximum number of 503 errors in the selected period.
* <b>Period</b>: Default value is 300 second.
  * <b>Recommended Values</b>:
    * <b>300 seconds</b> for near real-time monitoring.
    * <b>3600 seconds</b> for broader trend analysis over longer durations.

# Use Cases Example <a name="example"></a>
## Use Case 1: Service Maintenance or Scaling Issues <a name="example-1"></a>
Monitor 503 errors to detect periods of service maintenance or scaling issues that may result in temporary inability to handle incoming requests.



## Use Case 2: Load Balancer Performance Monitoring <a name="example-2"></a>
Use this metric to assess the load balancer's performance and ability to handle traffic without returning 503 errors, ensuring it is functioning as expected.



# Reference <a name="reference"></a>
* <b>Metrics Details</b>: https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-cloudwatch-metrics.html
* <b>AWS CloudWatch Parameters</b>: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/client/get_metric_data.html