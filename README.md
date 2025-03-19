# Cloudflare Automatic Dynamic DNS

CADDNS is an application that automatically updates the IP addresses of A records on Cloudflare to match the public IP of the machine it's running on. It seamlessly operates on Windows, Linux, and macOS, and can be executed using `npx caddns`, as it is available on npm packages.

## Features

- **Cross-Platform**: Works on Windows, Linux, and macOS.
- **Automated Updates**: Automatically updates Cloudflare DNS A records with the machine's public IP.
- **Easy Setup**: Initialize with `npx caddns` and receive help with every prompt.
- **Simple Configuration**: Manage records with intuitive options.
- **Automated Scheduling**: Runs daily tasks using cron jobs or Windows Task Scheduler.

## Installation

To install and run CADDNS, use npm:

```bash
npx caddns
```

## Setup

1. **Cloudflare Token**: Create a Cloudflare token with access to the desired DNS zone.
2. **Run Initial Setup**: 
- Launch CADDNS: `npx caddns`
- Input your Cloudflare token when prompted.
- Configure the DNS zone and select A records for IP updates.
3. **Automatic Configuration**: 
- CADDNS generates a config file in your user directory.
- Sets up a cron job or Windows task to run daily at midnight.

## Usage

Once configured, you can manage your settings by rerunning the script. You will be greeted with the following options:

- **Status**: View the current script version and active records.
- **Create New Configuration**: Delete existing configurations and create a new setup.
- **Add Record to Rule**: Add one or more records from the zone to the update rule.
- **Remove Record from Rule**: Remove one or more records from the update rule.
- **Remove All CADDNS Entries**: Delete all configurations and disable scheduled tasks.

## Documentation

Each action is documented within the script, providing guidance to ensure you know what you're doing with each step.

## Contributing

Contributions are welcome. Feel free to open PRs, create branches, etc..

## License

Under MIT license.
