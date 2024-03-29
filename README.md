# Java Periodic Report Generator

## Overview
This Java application is designed to demonstrate the use of `ScheduledExecutorService` for scheduling tasks that generate periodic reports. The program simulates a basic task that prints a message with a timestamp at regular intervals, showcasing how scheduled tasks can be managed in Java.

## Features
- **Periodic Task Scheduling**: Uses `ScheduledExecutorService` to schedule and execute tasks periodically.
- **Timestamps in Reports**: Each report includes a timestamp to illustrate the periodic nature of the task.
- **Customizable Frequency**: Currently configured to generate reports every 10 seconds, but can be adjusted as needed.

## How to Use
1. **Run the Application**: Execute the `Main` class.
2. **Observe the Output**: The program will print "Generating report..." along with the current timestamp every 10 seconds.
3. **Stop the Execution**: The program runs for a predefined duration (e.g., 50 seconds) and then gracefully shuts down the `ScheduledExecutorService`, terminating the report generation.

## Technical Implementation
- **ScheduledExecutorService**: Manages the scheduling and execution of the report generation task.
- **Runnable Task**: Defines the action to be executed periodically, which includes printing the report message with the current date and time.
- **Safe Shutdown**: Implements a proper shutdown process for the `ScheduledExecutorService` to ensure that all scheduled tasks are completed before the program exits.

## Running the Program
The program is pre-configured to run the task at a fixed rate of 10 seconds. Simply start the `Main` class, and the application will handle the scheduling and execution of tasks, followed by an automatic shutdown after 50 seconds.

## Purpose
This application serves as a practical example for those interested in learning how to use `ScheduledExecutorService` in Java for scheduling and executing tasks periodically. It's particularly useful for developers looking to implement scheduled tasks in their Java applications.

## Author
Made by Michal Frost

Happy coding.
```