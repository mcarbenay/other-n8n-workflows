# Workflow Documentation: 102_Send_updates_about_the_position_of_the_ISS_every_minute_to_a_topic_in_ActiveMQ

## Description
This workflow sends updates about the position of the ISS every minute to a topic in ActiveMQ.

## Nodes
1. **Cron**: Triggers the workflow every minute.
2. **HTTP Request**: Fetches the ISS position data.
3. **Set**: Formats the fetched data.

## Notes
- The ISS position data is retrieved from `https://api.wheretheiss.at/v1/satellites/25544/positions`.

---
