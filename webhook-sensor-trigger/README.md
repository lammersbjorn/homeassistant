# Webhook Trigger from Binary Sensor

This blueprint sends an HTTP POST webhook to a specified URL when a chosen binary sensor changes state.

**Before using this blueprint, add the following snippet to your configuration.yaml and restart HomeAssistant:**

```yaml
rest_command:
  send_webhook_request:
    url: "{{ url }}"
    method: POST
    payload: "{{ payload }}"
    content_type: "application/json
