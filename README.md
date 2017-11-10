# Shoryuken Upstart Script Example

It tooks me two days to setup the Shoryuken Upstart Script on our staging environment.

So I am sharing this examples to help others who may need it.

These scripts were inspired by the [Sidekiq Upstart script examples](https://github.com/mperham/sidekiq/blob/master/examples/upstart/sidekiq.conf).

If you are not familar with the Upstart script, I strongly recommend you make a quick walkthrough the [Upstart cookbook](http://upstart.ubuntu.com/cookbook).

# How to use it?

Copy shoryuken.conf and workers.conf to the /etc/init folder. change the `NUM_WORKERS` as you need. Set the uid & gid to your deploy username.

    # Start/stop a single Shoryuken
    $ start/stop shoryuken N=1
    or
    $ service shoryuken start/stop N=1

    # Start/stop or a set of Shoryuken instances
    $ start/stop workers
    or
    $ service workers start/stop

# Contributing

Bug reports and pull requests are welcome.
