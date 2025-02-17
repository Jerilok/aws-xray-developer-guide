# Monitoring endpoints and APIs with CloudWatch<a name="xray-services-cloudwatch"></a>

AWS X\-Ray integrates with Amazon CloudWatch to support CloudWatch ServiceLens, CloudWatch RUM, and CloudWatch Synthetics in monitoring the health of your applications\. By correlating metrics, logs, and traces, ServiceLens provides an end\-to\-end view of your services to help you quickly pinpoint performance bottlenecks and identify impacted users\. To learn more about ServiceLens, see [Using ServiceLens to Monitor the Health of Your Applications](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/ServiceLens.html)\.

With CloudWatch RUM, you can perform real user monitoring to collect and view client\-side data about your web application performance from actual user sessions in near\-real time\. With AWS X\-Ray and CloudWatch RUM, you can analyze and debug the request path starting from end users of your application through downstream AWS managed services\. This helps you identify latency trends and errors that impact your end users\. 

ServiceLens integrates with CloudWatch Synthetics, a fully managed service that you can use to monitor your endpoints and APIs from the outside in\. Synthetics uses modular, lightweight canaries that run 24 hours per day, once per minute\. Canaries are configurable scripts that follow the same routes and perform the same actions as a customer\. This enables the outside\-in view of your customers’ experiences, and your service’s availability from their point of view\. 

You can customize canaries to check for availability, latency, transactions, broken or dead links, step\-by\-step task completions, page load errors, load latency for UI assets, complex wizard flows, or other workflows in your application\.

To get started with Synthetics, enable X\-Ray for your APIs, endpoints, and web apps\. For example, you can do this for [your APIs running on API Gateway](xray-services-apigateway.md)\. Then, create a canary and observe the Synthetics node in your service graph\. To learn more about setting up Synthetics tests, see [Using Synthetics to Create and Manage Canaries](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Synthetics_Canaries.html)\.

**Topics**
+ [CloudWatch RUM and AWS X\-Ray](xray-services-RUM.md)
+ [Debugging CloudWatch synthetics canaries using X\-Ray](xray-services-cloudwatch-synthetics.md)