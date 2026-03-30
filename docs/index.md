# Continuous Intelligence

This site provides documentation for this project.
Use the navigation to explore module-specific materials.

## How-To Guide

Many instructions are common to all our projects.

See
[⭐ **Workflow: Apply Example**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get these projects running on your machine.

## Project Documentation Pages (docs/)

- **Home** - this documentation landing page
- **Project Instructions** - instructions specific to this module
- **Your Files** - how to copy the example and create your version
- **Glossary** - project terms and concepts

## Additional Resources

- [Suggested Datasets](https://denisecase.github.io/pro-analytics-02/reference/datasets/cintel/)


## Custom Project

### Dataset
The dataset used in this project was a modified version of the example dataset. I expanded it to 20 records to better simulate variation in system performance, particularly around response latency. This allowed for more meaningful testing of threshold-based signals.

### Signals
In addition to the original signals, I introduced a latency alert signal. This signal flags observations where the calculated average latency exceeds 30ms, assigning a value of 1 for high latency and 0 otherwise. This creates a simple but effective indicator for potential performance issues.

### Experiments
I modified the dataset by increasing the number of records and introducing a wider range of latency values. I also implemented a latency threshold signal to test how well it identifies high-latency scenarios. These changes were designed to evaluate how signal-based monitoring scales with more varied data.

### Results
The results were consistent with the original dataset but provided more visibility into latency patterns. The added records allowed the latency signal to trigger more frequently, highlighting cases where system performance exceeded acceptable thresholds.

### Interpretation
The introduction of a latency threshold signal shifts the analysis from descriptive to actionable. Instead of only observing latency values, the system now identifies when performance enters a risk state. With more records, the signal reveals patterns in when latency exceeds acceptable limits, which could indicate system strain under higher demand. This type of signal is valuable for real-time monitoring, alerting, and performance optimization, as it enables teams to respond proactively rather than reactively.
