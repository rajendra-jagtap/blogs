#    Amazon S3 Storage Lens – Organization-wide Visibility into Object Storage

## Introduction:

Amazon S3 Storage Lens provides a single view of object storage usage and activity across our entire Amazon S3 storage. It includes drilldown options to generate insights at the organization, account, Region, bucket, or even prefix level.
Amazon S3 Storage Lens aggregates our usage and activity metrics and displays the information in the account snapshot on the Amazon S3 console home (Buckets) page, interactive dashboards, or through a metrics export that we can download in CSV or Parquet format. We can use the dashboard to visualize insights and trends, flag outliers,and receive recommendations for optimizing storage costs and applying data protection best practices.

## How S3 Storage Lens works:

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens1.png?raw=true)

## Default Dashboard:

S3 Storage Lens includes an interactive dashboard which we can find in the S3 console. The dashboard gives us the ability to perform filtering and drill-down into our metrics to really understand how our storage is being used. The metrics are organized into categories like data protection and cost efficiency, to allow us to easily find relevant metrics.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens2.png?raw=true)

## Creating a Dashboard:

We can also create our own dashboards from scratch, to do this I head over to the S3 console and click on the Dashboards menu item inside the Storage Lens section. Secondly, I click the Create dashboard button.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens3.png?raw=true)

I give my dashboard the name lens-demo-dashboard and select a home Region. The home Region is where the metrics data for our dashboard will be stored. I choose to enable the dashboard, meaning that it will be updated daily with new metrics.
A dashboard can analyze storage across accounts, Regions, buckets, and prefix. I choose to include all buckets from my account and across all regions in the Dashboard scope section

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens4.png?raw=true)


S3 Storage Lens has two tiers: Free Metrics, which is free of charge, automatically available for all S3 customers and contains 15 usage related metrics; and Advanced metrics and recommendations, which has an additional charge, but includes all 29 usage and activity metrics with 15-month data retention, and contextual recommendations.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens5.png?raw=true)

## What does a Dashboard Show :
Once our dashboard has been created, we can start to explore the data. We can filter by Accounts, Regions, Storage classes, Buckets, and Prefixes at the top of the dashboard.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens6.png?raw=true)

The next section is a snapshot of the metrics such as the Total storage and Object count, and we can see a trend line that shows the trend on each metric over the last 30 days and a percentage change. The number in the % change column shows by default the Day/day percentage change, but we can select to compare by Week/week or Month/month.
We can toggle between different Metric groups by selecting either Summary, Cost efficiency, Data protection, or Activity.
There are some metrics here that are pretty typical like total storage and object counts, and we can already receive these in a few places in the S3 console and in Amazon CloudWatch – but in S3 Storage Lens we can receive these metrics in aggregate across our organization or account, or at the prefix level, which was not previously possible.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens7.png?raw=true)

The dashboard trends and distribution section allows me to compare two metrics over time in more detail. Here I have selected Total storage as my Primary metric and Object Count as my Secondary metric.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens8.png?raw=true)

The dashboard also shows us those two metrics and how they are distributed across Storage class and Regions.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens9.png?raw=true)

The last section of the dashboard allows us to perform a Top N analysis of a metric over a date range, where N is between 1 and 25. In the example below, we have selected the top 3 items in descending order for the Total storage metric.

![alt text](https://github.com/rajendra-jagtap/blogs/blob/main/images/lens/lens10.png?raw=true)
