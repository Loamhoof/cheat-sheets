Index
-----

* [Shell](#shell)

Shell
-----

Basic commands:
* `list_queues` to display the number of messages in each queue
* `list_consumers` to display the active consumers
* `purge_queue <queue>` to purge a queue

Admin commands (require [rabbitmqadmin](https://www.rabbitmq.com/management-cli.html)):
* `get queue=<queue> requeue=true [...]` to display the content of a queue

Other:
* Purge all queues: `rabbitmqctl list_queues | grep -oP '^\w+(?=\D+\d)' | xargs -n 1 rabbitmqctl purge_queue`
