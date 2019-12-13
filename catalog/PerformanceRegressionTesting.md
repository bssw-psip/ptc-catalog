# Performance Regression Testing

## Target

To develop test suites that exercise performance capabilities and plans for how to make practical use of that performance data.

## User Story

As a project lead, I want to be able to identify when changes to the code introduces performance issues so that we can 
address them sooner rather than later in the development process.

## Card

| Score         | Description |
| :-------------: | :------------- |
| 0 | No performance regression testing. |
| 1 | A testable primary use case and set of measurements that are important to performance are established. |
| 2 | One or more test cases that exercise the performance capability according to the measurements are created. |
| 3 | The performance history of the tests are tracked over time. |
| 4 | Performance tracking is run at regular intervals on relevant platforms. |
| 5 | Team commits to reviewing the performance tracking information.|

## Comments

- Performance regression testing means knowing about the past, being able to run something fairly easily to check 
performance, to detect negative or positive changes.
- Measurements can include wall clock time, resource utilization, cache performance, scalability, correctness, 
and others. The choice of measurements will inform the test(s) that need to be written.
- A performance test should be able to be checked relatively easily yet it is one that also exercises the code adequately.
- Bonus steps in this PTC might include repeating these steps to support a another use case, set of measurements, 
and/or more tests.
