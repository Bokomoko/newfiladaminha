# Queue Entity

The Queue entity represents a queue with the following attributes:

## Attributes

| Attribute       | Type                | Description                                                                 |
|-----------------|---------------------|-----------------------------------------------------------------------------|
| id              | String              | A unique identifier for the queue.                                          |
| creation_date   | Date                | The date when the queue was created.                                        |
| expiration_date | Date                | The date when the queue will expire. This is obtained by default from the parameters. |
| owner_id        | String              | The identifier of the owner of the queue.                                   |
| queued-items    | Array of 1000 items | An array of 1000 positions, initially empty, containing queue items. Each queue item is described in the [queue-items-entity.md](./queue-items-entity.md) file. |
| last_position   | Integer             | The last position in the queue, initialized with 0.                         |
