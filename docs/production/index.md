# Production

This section contains information about HCB's production environment, deployment processes, and operational considerations.

## Deployment

HCB is deployed on [Heroku](https://www.heroku.com/). We have two dynos, one for Rails and one for our [Sidekiq](https://github.com/sidekiq/sidekiq) workers.

## Monitoring

We use several tools to monitor HCB in production:

- [Airbrake](https://www.airbrake.io/) for error tracking
- [AppSignal](https://www.appsignal.com/) for performance monitoring
- [Checkly](https://www.checklyhq.com/) for running [status.hackclub.com](https://status.hackclub.com/)

## Infrastructure

More information about HCB's production infrastructure will be added here in the future.
