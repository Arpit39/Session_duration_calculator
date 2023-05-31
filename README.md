# Log File Processing

This Python script processes a log file containing user session information and calculates the total time spent by each user in their sessions.

## Prerequisites

- Python 3.x

## Usage

1. Make sure you have Python installed on your system.

2. Open a terminal or command prompt.

3. Run the script with the log file as a command-line argument:

```python script.py <log_file>```


Replace `<log_file>` with the path to your log file.

4. The script will process the log file and display the total session count and time spent for each user.

## Input Format

The log file should be a plain text file with each line representing a log entry. Each log entry should have the following format:

```<timestamp> <user> <action>```


- `<timestamp>`: The timestamp of the log entry in the format `HH:MM:SS`.
- `<user>`: The user identifier.
- `<action>`: Either "Start" or "End" to indicate the start or end of a user session.

Example log file:

14:02:03 ALICE99 Start
14:02:05 CHARLIE End
14:02:34 ALICE99 End
14:02:58 ALICE99 Start
14:03:02 CHARLIE Start
14:03:33 ALICE99 Start
14:03:35 ALICE99 End
14:03:37 CHARLIE End
14:04:05 ALICE99 End
14:04:23 ALICE99 End
14:04:41 CHARLIE Start


## Output

The script will calculate the total session count and time spent for each user and display the results in ascending order of user identifiers. The output format for each user is as follows:

```<user> <session_count> <total_time>```


- `<user>`: The user identifier.
- `<session_count>`: The total number of sessions for the user.
- `<total_time>`: The total time spent by the user in seconds.

Example output:

ALICE99 4 240
CHARLIE 3 37
