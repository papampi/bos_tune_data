# Braiins OS+ Tuner Bash Script

This is a Bash script for monitoring and tuning Braiins OS+ miners using the Braiins BOS+ API. The script retrieves the miner's power target, hash rate, power consumption, and efficiency, and prints the data in a table format.

## Prerequisites

- Bash shell
- [grpcurl ↗](https://github.com/fullstorydev/grpcurl) command-line tool
- Access to the Braiins BOS+ API with a valid authorization token

## Usage

To use the script, run it with the IP address of the miner as the first command-line argument:

```
./bos-tuner.sh <IP_ADDRESS>
```

Replace `<IP_ADDRESS>` with the IP address of your miner.

## Configuration

Before running the script, you need to set the miner's username and password in the script:

```
USERNAME="root"
PASSWORD="root"
```

## Output

The script outputs a table with the following columns:

- Power Target: the miner's power target in watts
- Hash Rate TH/s: the miner's hash rate in terahashes per second (TH/s)
- Power Consumption: the miner's estimated power consumption in watts
- Efficiency: the miner's efficiency in joules per terahash (J/TH)

The table is formatted for easy readability and alignment using the `printf` command.

## Contributing

If you find a bug or have a suggestion for improvement, feel free to open an issue or submit a pull request.

## License

This script is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
