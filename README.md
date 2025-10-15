### 💼 Project Title

Load & Stress Testing of Foodi Web Launching Page using Jmeter.

### 📝 Project Description

This project focuses on performing Load and Stress Testing on the Foodi Web Launching Page using Apache JMeter to analyze its performance, reliability, and scalability under varying user loads. The goal is to ensure that the website can handle expected and peak traffic efficiently without performance degradation or downtime.  
The Foodi website is an online food ordering platform where users can browse, sign up, and explore restaurants. This test aims to evaluate how the web launching (home) page responds when multiple users access it simultaneously.


### 🎯 Project Objectives

- To determine the maximum number of concurrent users the Foodi launching page can handle.

- To measure response time, throughput, and error percentage under load.

- To identify potential performance bottlenecks and system breaking points.

- To verify system stability and responsiveness under stress conditions.

### 🎥 Project Video Link

```
https://drive.google.com/file/d/1jzR0XpiO5VeMQ3X6OO1w77XU4qpShRC6/view?usp=sharing
```

### 🔗 Foodi Web Launching Page URL

```
https://foodibd.com
```

### 🧰 Tools & Technologies

- Tool Used: Apache JMeter

- Version: 5.x

- Protocol: HTTP(S)

- Test Type: Load & Stress Testing

### 🗂️ Project Structure

```
│  
└── Test Plan # Main container  
└── Thread Group # For create virtual user  
└── Header Manager # Add Header info  
└── Sampler # For sending request to server  
└── Timer # Add delay between request  
└── Assertion # Check the Response or Request  
└── Listener # View Results
```

### 🔎 Observations

1. **Test data:**

    - Total number of users or samples: 1000
    - Total samples: 953
    - Ramp-up period: 3

    - Expected & Actual Results Info: 

        - Expected Result: At a time 1000 users should access the launching page of foodi web within 3 sec of Ramp-up period.
        - Actual Result: At a time 953 users should access the launching page of foodi web within 3 sec of Ramp-up period but response time decreases and user can't load after 953 users or samples.  

2. **Performance Test Results Report**

    - Average Response Time: 8512 ms
    - Throughput (/sec): 29.2/sec
    - Error Rate (%): 4.62%

### 🏁 Conclusion

The Load and Stress Testing successfully evaluated the stability, scalability, and performance limits of the Foodi Web Launching Page.  
Findings from this test will help improve the website's server configuration, response optimization, and user experience during high-traffic events such as promotions or new feature releases.

