# Queue Item Entity

The `Queue Item Entity` represents an item in the queue. It is a child of the [Queue Entity](queue-entity.md).

## Attributes

- **user_id**: The ID of the user who joined the queue.
- **timestamp**: The timestamp when the user joined the queue.
- **flag**: A flag indicating the status or priority of the queue item.
- **original_position**: The original position of the user in the queue.
- **queue_id**: The ID of the queue to which this item belongs.

```json
{
  "user_id": "string",
  "timestamp": "string",
  "flag": "boolean",
  "original_position": "integer",
  "queue_id": "string"
}
```
