# Load-and-Stress-Testing-on-Foodie-App

Load Testing and Stress Testing are two important types of performance testing used in software quality assurance (SQA) to evaluate how a system behaves under specific conditions. Here's a simple explanation of each:

🔸 **Load Testing**
Purpose: To check how the system performs under expected or typical user loads.

Goal: Identify performance bottlenecks (e.g., slow response times) before the system goes live.

Example: Testing an e-commerce website with 500 users placing orders simultaneously to see if the system can handle it efficiently.

🔸 **Stress Testing**
Purpose: To check how the system performs beyond its limits or under extreme conditions.

Goal: Determine the system’s breaking point and how it recovers from failure.

Example: Testing a ticket booking site by continuously increasing users (1000 → 2000 → 3000+) until it crashes.

Load and stress testing help ensure software reliability and performance by identifying system behavior under normal and extreme conditions. They detect bottlenecks, measure response times, and validate scalability. This improves user experience, prevents crashes, and supports informed capacity planning.

I performed load and stress testing on "Foodie App" using Jmeter software where I used ->
- Thread Group
- Sampler (Where I choose the HTTP Request and used Both Get and Post method)
- Timer (Constant Timer and Uniform Random Timer)
- Logic Controller (Loop Count)
- Listener (View Results in Table)

I created three Thread Groups, one Loop Controller, one Constant Timer, one Uniform Random Timer, and six HTTP Requests. I configured 2 HTTP Requests per thread. The first thread also includes a Logic Controller for one HTTP Request and a listener (View Results in Table) to view the results. The second thread has two listeners (View Results in Table) for its two HTTP Requests. The third thread includes a Constant Timer and a Uniform Random Timer. I set the Number of Threads, Ramp-Up Period, Loop Count, Timers, and Loop Controller for all three threads. Finally, I added a listener (View Results in Table) to analyze the overall results. During analysis, a total of 1,525 users hit the application as per the environment setup, but the system stopped after 1,481 user hits.  


