# Queue Entity

The Queue entity represents a queue with the following attributes:

- **id**: A unique identifier for the queue.
- **creation_date**: The date when the queue was created.
- **expiration_date**: The date when the queue will expire. This is obtained by default from the parameters.
- **owner_id**: The identifier of the owner of the queue.
- **queued-items**: An array of 1000 positions, initially empty, containing queue items. Each queue item is described in the [queue-items-entity.md](./queue-items-entity.md) file.
- **last_position**: The last position in the queue, initialized with 0.

## Attributes

### id
- **Type**: String
- **Description**: A unique identifier for the queue.

### creation_date
- **Type**: Date
- **Description**: The date when the queue was created.

### expiration_date
- **Type**: Date
- **Description**: The date when the queue will expire. This is obtained by default from the parameters.

### owner_id
- **Type**: String
- **Description**: The identifier of the owner of the queue.

### queued-items
- **Type**: Array of 1000 positions
- **Description**: An array of 1000 positions, initially empty, containing queue items. Each queue item is described in the [queue-items-entity.md](./queue-items-entity.md) file.

### last_position
- **Type**: Integer
- **Description**: The last position in the queue, initialized with 0.
